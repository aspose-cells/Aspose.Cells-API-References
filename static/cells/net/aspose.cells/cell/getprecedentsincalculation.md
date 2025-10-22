##Cell.GetPrecedentsInCalculation
Cell method. Gets all precedentsreference to cells in current workbook used by this cells formula while calculating it
## Cell.GetPrecedentsInCalculation method
Gets all precedents(reference to cells in current workbook) used by this cell's formula while calculating it.
```csharp
public IEnumerator GetPrecedentsInCalculation()
```
### Return Value
Enumerator to enumerate all references(ReferredArea)
### Remarks
This method can only work with the situation that [`EnableCalculationChain`](../../formulasettings/enablecalculationchain/) is true for the workbook and the workbook has been fully calculated. If this cell is not a formula or it does not reference to any other cells, null will be returned.
### Examples
```csharp
using System;
using System.Collections;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellMethodGetPrecedentsInCalculationDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Cells cells = workbook.Worksheets[0].Cells;
cells["B1"].PutValue(10);
cells["B2"].PutValue(20);
cells["A2"].Formula = "=IF(TRUE,B2,B1)";
workbook.Settings.FormulaSettings.EnableCalculationChain = true;
workbook.CalculateFormula();
IEnumerator en = cells["A2"].GetPrecedentsInCalculation();
Console.WriteLine("A2's calculation precedents:");
while(en.MoveNext())
{
ReferredArea r = (ReferredArea)en.Current;
Console.WriteLine(r);
}
}
}
}
```
### See Also
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
