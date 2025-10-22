##Cell.GetPrecedents
Cell method. Gets all references appearing in this cells formula
## Cell.GetPrecedents method
Gets all references appearing in this cell's formula.
```csharp
public ReferredAreaCollection GetPrecedents()
```
### Return Value
Collection of all references appearing in this cell's formula.
### Remarks
Returns null if this is not a formula cell.All references appearing in this cell's formula will be returned no matter they are referenced or not while calculating. For example, although cell A2 in formula "=IF(TRUE,A1,A2)" is not used while calculating, it is still taken as the formula's precedents.To get those references which influence the calculation only, please use [`GetPrecedentsInCalculation`](../getprecedentsincalculation/).
### Examples
```csharp
using System;
using System.Text;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellMethodGetPrecedentsDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Cells cells = workbook.Worksheets[0].Cells;
// Set formula with precedents
cells["A1"].Formula = "=B1+SUM(B1:B10)+[Book1.xls]Sheet1!A1";
// Get all precedent references
ReferredAreaCollection areas = cells["A1"].GetPrecedents();
// Display each precedent reference
foreach (ReferredArea area in areas)
{
StringBuilder sb = new StringBuilder();
if (area.IsExternalLink)
{
sb.Append($"[{area.ExternalFileName}]");
}
sb.Append($"{area.SheetName}!");
sb.Append(CellsHelper.CellIndexToName(area.StartRow, area.StartColumn));
if (area.IsArea)
{
sb.Append($":{CellsHelper.CellIndexToName(area.EndRow, area.EndColumn)}");
}
Console.WriteLine(sb.ToString());
}
}
}
}
```
### See Also
* class [ReferredAreaCollection](../../referredareacollection/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
