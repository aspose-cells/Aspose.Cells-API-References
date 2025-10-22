##Cells.GetDependents
Cells method. Get all cells which refer to the specific cell
## Cells.GetDependents method
Get all cells which refer to the specific cell.
```csharp
public Cell[] GetDependents(bool isAll, int row, int column)
```
| Parameter | Type | Description |
| --- | --- | --- |
| isAll | Boolean | Indicates whether check other worksheets |
| row | Int32 | The row index. |
| column | Int32 | The column index. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsMethodGetDependentsWithBooleanInt32Int32Demo
{
public static void Run()
{
// Create a workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Set up sample formulas and values
cells["A1"].PutValue(10);
cells["B1"].Formula = "=A1*2";
cells["C1"].Formula = "=A1+B1";
cells["D1"].Formula = "=B1*3";
cells["F4"].Formula = "=A1*5";
// Calculate formulas
workbook.CalculateFormula();
// Get direct dependents of cell A1 (row 0, column 0)
Cell[] directDependents = cells.GetDependents(false, 0, 0);
Console.WriteLine("Direct dependents of A1:");
foreach (Cell cell in directDependents)
{
Console.WriteLine(cell.Name);
}
// Get all dependents (including indirect) of cell A1 (row 0, column 0)
Cell[] allDependents = cells.GetDependents(true, 0, 0);
Console.WriteLine("\nAll dependents of A1:");
foreach (Cell cell in allDependents)
{
Console.WriteLine(cell.Name);
}
}
}
}
```
### See Also
* class [Cell](../../cell/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
