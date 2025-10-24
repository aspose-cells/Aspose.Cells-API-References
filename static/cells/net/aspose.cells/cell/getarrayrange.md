##Cell.GetArrayRange
Cell method. Gets the array range if the cells formula is an array formula
## Cell.GetArrayRange method
Gets the array range if the cell's formula is an array formula.
```csharp
public CellArea GetArrayRange()
```
### Return Value
The array range.
### Remarks
Only applies when the cell's formula is an array formula
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellMethodGetArrayRangeDemo
{
public static void Run()
{
// Create a workbook
Workbook wb = new Workbook();
Cells cells = wb.Worksheets[0].Cells;
// Set a dynamic array formula in cell A1
Cell cell = cells[0, 0];
string formula = "=SEQUENCE(3,2)";
cell.SetDynamicArrayFormula(formula, new FormulaParseOptions(), false);
// Calculate formulas
wb.CalculateFormula();
// Get the array range of the dynamic formula
CellArea arrayRange = cell.GetArrayRange();
// Output the array range information
Console.WriteLine("Array range for dynamic formula:");
Console.WriteLine($"Start row: {arrayRange.StartRow}");
Console.WriteLine($"Start column: {arrayRange.StartColumn}");
Console.WriteLine($"End row: {arrayRange.EndRow}");
Console.WriteLine($"End column: {arrayRange.EndColumn}");
// Print the values in the array range
Console.WriteLine("\nValues in the array range:");
for (int r = arrayRange.StartRow; r <= arrayRange.EndRow; r++)
{
for (int c = arrayRange.StartColumn; c <= arrayRange.EndColumn; c++)
{
Console.Write(cells[r, c].Value + "\t");
}
Console.WriteLine();
}
}
}
}
```
### See Also
* struct [CellArea](../../cellarea/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
