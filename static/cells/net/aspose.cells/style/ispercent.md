##Style.IsPercent
Style property. Indicates whether the number format is a percent format
## Style.IsPercent property
Indicates whether the number format is a percent format.
```csharp
public bool IsPercent { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class StylePropertyIsPercentDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Access cell A1 and set its value
Cell cell = worksheet.Cells["A1"];
cell.PutValue(0.5);
// Get the style of the cell
Style style = cell.GetStyle();
// Display current IsPercent value
Console.WriteLine("Current IsPercent value: " + style.IsPercent);
// Set number format to percentage (this will automatically set IsPercent to true)
style.Number = 10; // 10 is the built-in percentage format in Excel
// Apply the style to the cell
cell.SetStyle(style);
// Verify IsPercent is now true
Console.WriteLine("After setting percentage format, IsPercent value: " + style.IsPercent);
// Create another cell with different format
Cell cell2 = worksheet.Cells["A2"];
cell2.PutValue(0.75);
Style style2 = cell2.GetStyle();
style2.Number = 3; // 3 is the built-in number format (not percentage)
cell2.SetStyle(style2);
// Verify IsPercent is false for non-percentage format
Console.WriteLine("For non-percentage format, IsPercent value: " + style2.IsPercent);
// Save the workbook
workbook.Save("StylePropertyIsPercentDemo.xlsx");
}
}
}
```
### See Also
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
