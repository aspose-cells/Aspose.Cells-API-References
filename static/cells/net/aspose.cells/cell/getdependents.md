##Cell.GetDependents
Cell method. Get all cells whose formula references to this cell directly
## Cell.GetDependents method
Get all cells whose formula references to this cell directly.
```csharp
public Cell[] GetDependents(bool isAll)
```
| Parameter | Type | Description |
| --- | --- | --- |
| isAll | Boolean | Indicates whether check formulas in other worksheets |
### Remarks
If one reference containing this cell appears in one cell's formula, that cell will be taken as the dependent of this cell, no matter the reference or this cell is used or not while calculating. For example, although cell A2 in formula "=IF(TRUE,A1,A2)" is not used while calculating, this formula is still be taken as A2's dependent. To get those formulas whose calculated results depend on this cell, please use [`GetDependentsInCalculation`](../getdependentsincalculation/).When tracing dependents for one cell, all formulas in the workbook or worksheet will be analized and checked. So it is a time consumed process. If user need to trace dependents for lots of cells, using this method will cause poor performance. For performance consideration, user should use [`GetDependentsInCalculation`](../getdependentsincalculation/) instead. Or, user may gather precedents map of all cells by [`GetPrecedents`](../getprecedents/) firstly, and then build the dependents map according to the precedents map.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellMethodGetDependentsWithBooleanDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Set formulas that reference B1
cells["A1"].Formula = "=B1+5";
cells["A2"].Formula = "=B1*2";
cells["A3"].Formula = "=SUM(B1:B3)";
// Calculate formulas
workbook.CalculateFormula();
// Get all cells that depend on B1 (recursive)
Cell[] dependents = cells["B1"].GetDependents(true);
Console.WriteLine("Cells dependent on B1:");
foreach (Cell cell in dependents)
{
Console.WriteLine(cell.Name + ": " + cell.Formula);
}
}
}
}
```
### See Also
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
