##Cell.StringValue
Cell property. Gets the string value contained in the cell. If the type of this cell is string then return the string value itself. For other cell types the formatted string value formatted with the specified style of this cell will be returned. The formatted cell value is same with what you can get from excel when copying a cell as textsuch as copying cell to text editor or exporting to csv
## Cell.StringValue property
Gets the string value contained in the cell. If the type of this cell is string, then return the string value itself. For other cell types, the formatted string value (formatted with the specified style of this cell) will be returned. The formatted cell value is same with what you can get from excel when copying a cell as text(such as copying cell to text editor or exporting to csv).
```csharp
public string StringValue { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellPropertyStringValueDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Set some values
cells["A1"].PutValue("Hello");
cells["A2"].PutValue(123);
cells["A3"].PutValue(DateTime.Now);
cells["A4"].Formula = "=A1&A2";
// Calculate formulas
workbook.CalculateFormula();
// Demonstrate StringValue property
Console.WriteLine("A1 StringValue: " + cells["A1"].StringValue);
Console.WriteLine("A2 StringValue: " + cells["A2"].StringValue);
Console.WriteLine("A3 StringValue: " + cells["A3"].StringValue);
Console.WriteLine("A4 StringValue: " + cells["A4"].StringValue);
// Show error value case
Cell errorCell = cells["B1"];
errorCell.Formula = "=1/0";
workbook.CalculateFormula();
Console.WriteLine("B1 (Error) StringValue: " + errorCell.StringValue);
}
}
}
```
### See Also
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
