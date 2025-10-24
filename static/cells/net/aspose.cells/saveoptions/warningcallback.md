##SaveOptions.WarningCallback
SaveOptions property. Gets or sets warning callback
## SaveOptions.WarningCallback property
Gets or sets warning callback.
```csharp
public IWarningCallback WarningCallback { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class SaveOptionsPropertyWarningCallbackDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Sample data");
// Create save options
HtmlSaveOptions saveOptions = new HtmlSaveOptions();
// Set custom warning callback
saveOptions.WarningCallback = new CustomWarningCallback();
// This will generate a warning about unsupported feature in HTML format
worksheet.PageSetup.PrintTitleRows = "$1:$1";
// Save with options that might trigger warnings
workbook.Save("WarningCallbackDemo.html", saveOptions);
}
}
public class CustomWarningCallback : IWarningCallback
{
public void Warning(WarningInfo warningInfo)
{
// Handle the warning - in this case just display it
Console.WriteLine($"Warning: {warningInfo.Description}");
Console.WriteLine($"Warning type: {warningInfo.WarningType}");
}
}
}
```
### See Also
* interface [IWarningCallback](../../iwarningcallback/)
* class [SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
