##Cell.GetDependentsInCalculation
Cell method. Gets all cells whose calculated result depends on this cell
## Cell.GetDependentsInCalculation method
Gets all cells whose calculated result depends on this cell.
```csharp
public IEnumerator GetDependentsInCalculation(bool recursive)
```
| Parameter | Type | Description |
| --- | --- | --- |
| recursive | Boolean | Whether returns those dependents which do not reference to this cell directly but reference to other leafs of this cell |
### Return Value
Enumerator to enumerate all dependents(Cell objects)
### Remarks
To use this method, please make sure the workbook has been set with true value for [`EnableCalculationChain`](../../formulasettings/enablecalculationchain/) and has been fully calculated with this setting. If there is no formula reference to this cell, null will be returned.
### Examples
```csharp
using System;
using System.Collections;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellMethodGetDependentsInCalculationWithBooleanDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Cells cells = workbook.Worksheets[0].Cells;
cells["A1"].Formula = "=B1+SUM(B1:B10)+[Book1.xls]Sheet1!B2";
cells["A2"].Formula = "=IF(TRUE,B2,B1)";
workbook.Settings.FormulaSettings.EnableCalculationChain = true;
workbook.CalculateFormula();
IEnumerator en = cells["B1"].GetDependentsInCalculation(false);
Console.WriteLine("B1's calculation dependents:");
while(en.MoveNext())
{
Cell c = (Cell)en.Current;
Console.WriteLine(c.Name);
}
en = cells["B2"].GetDependentsInCalculation(false);
Console.WriteLine("B2's calculation dependents:");
while(en.MoveNext())
{
Cell c = (Cell)en.Current;
Console.WriteLine(c.Name);
}
}
}
}
```
### See Also
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
