##ReferredArea.EndRow
ReferredArea property. The end row of the area
## ReferredArea.EndRow property
The end row of the area.
```csharp
public int EndRow { get; }
```
### Examples
```csharp
using System;
using System.Text;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ReferredAreaPropertyEndRowDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Cells cells = workbook.Worksheets[0].Cells;
// Set formula with multiple references
cells["A1"].Formula = "= B1 + SUM(B1:B10) + [Book1.xls]Sheet1!A1";
// Get all precedent areas
ReferredAreaCollection areas = cells["A1"].GetPrecedents();
// Process each reference
foreach (ReferredArea area in areas)
{
StringBuilder sb = new StringBuilder();
if (area.IsExternalLink)
{
sb.Append($"[{area.ExternalFileName}]");
}
sb.Append($"{area.SheetName}!");
sb.Append(CellsHelper.CellIndexToName(area.StartRow, area.StartColumn));
// Demonstrate EndRow usage for range references
if (area.IsArea)
{
sb.Append($":{CellsHelper.CellIndexToName(area.EndRow, area.EndColumn)}");
}
Console.WriteLine(sb.ToString());
}
workbook.Save("ReferredAreaExample.xlsx");
}
}
}
```
### See Also
* class [ReferredArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
