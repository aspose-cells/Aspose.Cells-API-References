##LoadOptions.WarningCallback
LoadOptions property. Gets or sets warning callback
## LoadOptions.WarningCallback property
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
public class CustomWarningCallback : IWarningCallback
{
public void Warning(WarningInfo warningInfo)
{
Console.WriteLine($"Warning: {warningInfo.Description}");
}
}
public class LoadOptionsPropertyWarningCallbackDemo
{
public static void Run()
{
// Create a custom warning callback
IWarningCallback warningCallback = new CustomWarningCallback();
// Initialize load options with warning callback
LoadOptions options = new LoadOptions();
options.WarningCallback = warningCallback;
options.IgnoreUselessShapes = true;
// Load workbook with options
Workbook workbook = new Workbook("example.xlsx", options);
// Demonstrate warning callback usage by accessing a cell
Console.WriteLine($"Cell value: {workbook.Worksheets[0].Cells["A1"].StringValue}");
// Save the workbook
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* interface [IWarningCallback](../../iwarningcallback/)
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
