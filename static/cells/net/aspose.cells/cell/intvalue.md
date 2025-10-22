##Cell.IntValue
Cell property. Gets the integer value contained in the cell
## Cell.IntValue property
Gets the integer value contained in the cell.
```csharp
public int IntValue { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellPropertyIntValueDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Cells cells = workbook.Worksheets[0].Cells;
// Set a numeric value and get IntValue
Cell cell1 = cells[0, 0];
cell1.PutValue(42);
Console.WriteLine("IntValue of numeric cell: " + cell1.IntValue);
// Set a formula that evaluates to a number and get IntValue
Cell cell2 = cells[0, 1];
cell2.Formula = "=10+5";
workbook.CalculateFormula();
Console.WriteLine("IntValue of formula cell: " + cell2.IntValue);
// Set a boolean value and get IntValue
Cell cell3 = cells[0, 2];
cell3.PutValue(true);
Console.WriteLine("IntValue of boolean cell: " + cell3.IntValue);
// Set a text value and get IntValue (will be 0 if not convertible)
Cell cell4 = cells[0, 3];
cell4.PutValue("Hello");
Console.WriteLine("IntValue of text cell: " + cell4.IntValue);
}
}
}
```
### See Also
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
