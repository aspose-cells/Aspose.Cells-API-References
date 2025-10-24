##HtmlLoadOptions.HtmlLoadOptions
HtmlLoadOptions constructor. Creates an options of loading the file
## HtmlLoadOptions() {#constructor}
Creates an options of loading the file.
```csharp
public HtmlLoadOptions()
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class HtmlLoadOptionsMethodCtorDemo
{
public static void Run()
{
// Create HTML load options using constructor
HtmlLoadOptions loadOptions = new HtmlLoadOptions();
loadOptions.SupportDivTag = true;
// Load HTML file with the options
Workbook workbook = new Workbook("example.html", loadOptions);
// Access data from the loaded HTML
Worksheet worksheet = workbook.Worksheets[0];
Console.WriteLine("B1 Cell Value: " + worksheet.Cells["B1"].StringValue);
Console.WriteLine("B3 Cell Value: " + worksheet.Cells["B3"].StringValue);
Console.WriteLine("B4 Cell Value: " + worksheet.Cells["B4"].StringValue);
}
}
}
```
### See Also
* class [HtmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## HtmlLoadOptions(LoadFormat) {#constructor_1}
Creates an options of loading the file.
```csharp
public HtmlLoadOptions(LoadFormat loadFormat)
```
| Parameter | Type | Description |
| --- | --- | --- |
| loadFormat | LoadFormat | The loading format. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class HtmlLoadOptionsMethodCtorWithLoadFormatDemo
{
public static void Run()
{
try
{
// Create HtmlLoadOptions instance using constructor with LoadFormat parameter
HtmlLoadOptions loadOptions = new HtmlLoadOptions(LoadFormat.Html);
// Set some properties of the HtmlLoadOptions
loadOptions.AutoFitColsAndRows = true;
loadOptions.SupportDivTag = true;
loadOptions.DeleteRedundantSpaces = true;
// Create a workbook using the load options
Workbook workbook = new Workbook("input.html", loadOptions);
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Display some information about the loaded HTML
Console.WriteLine("HTML loaded successfully with LoadFormat.Html");
Console.WriteLine($"Worksheet name: {worksheet.Name}");
Console.WriteLine($"Cells count: {worksheet.Cells.MaxDataRow + 1} rows x {worksheet.Cells.MaxDataColumn + 1} columns");
// Save the workbook
workbook.Save("HtmlLoadOptionsCtorDemo.xlsx");
}
catch (Exception ex)
{
Console.WriteLine($"Error loading HTML file: {ex.Message}");
}
}
}
}
```
### See Also
* enum [LoadFormat](../../loadformat/)
* class [HtmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
