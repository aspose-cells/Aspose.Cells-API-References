##Cell.DisplayStringValue
Cell property. Gets the formatted string value of this cell by cells display style
## Cell.DisplayStringValue property
Gets the formatted string value of this cell by cell's display style.
```csharp
public string DisplayStringValue { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellPropertyDisplayStringValueDemo
{
public static void Run()
{
Workbook wb = new Workbook();
Worksheet sheet = wb.Worksheets[0];
Cell cell = sheet.Cells[0, 0];
// First example
Style style = cell.GetStyle();
style.Custom = "# ##/##\\\"";
cell.SetStyle(style);
cell.PutValue(3);
Console.WriteLine("DisplayStringValue: " + cell.DisplayStringValue); // Output: 3"
// Second example
style.Custom = "\"a\"#\"b\" \"c\"##\"d\"/\"e\"##";
cell.SetStyle(style);
Console.WriteLine("DisplayStringValue: " + cell.DisplayStringValue); // Output: a3
// Third example
style.Custom = "\"a\"#\"b\" \"c\"##\"d\"/\"e\"##\"f\"";
cell.SetStyle(style);
Console.WriteLine("DisplayStringValue: " + cell.DisplayStringValue); // Output: a3f
// Fourth example with decimal value
cell.PutValue(1.234);
Console.WriteLine("DisplayStringValue: " + cell.DisplayStringValue); // Output: a1b c11d/e47f
// Fifth example with modified format
style.Custom = "\"a\"#\"b\"\"c\"##\"d\"/\"e\"##\"f\"";
cell.SetStyle(style);
cell.PutValue(3);
Console.WriteLine("DisplayStringValue: " + cell.DisplayStringValue); // Output: a3f
// Sixth example with decimal value
cell.PutValue(1.234);
Console.WriteLine("DisplayStringValue: " + cell.DisplayStringValue); // Output: a1bc11d/e47f
}
}
}
```
### See Also
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
