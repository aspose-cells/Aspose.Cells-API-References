##ReferredArea.IsArea
ReferredArea property. Indicates whether this is an area
## ReferredArea.IsArea property
Indicates whether this is an area.
```csharp
public bool IsArea { get; }
```
### Remarks
If this is not an area, only StartRow and StartColumn effect.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ReferredAreaPropertyIsAreaDemo
{
public static void Run()
{
Workbook wb = new Workbook();
Name n = wb.Worksheets.Names[wb.Worksheets.Names.Add("testname")];
n.RefersTo = "=Sheet1!$A$1:$B$2,Sheet1!$C$3,Sheet2!$D$4,Sheet1!E5";
ReferredArea[] referredAreas = n.GetReferredAreas(true);
Console.WriteLine("Referred Areas Count: " + referredAreas.Length);
Console.WriteLine();
for (int i = 0; i < referredAreas.Length; i++)
{
ReferredArea ra = referredAreas[i];
Console.WriteLine($"Area {i + 1}:");
Console.WriteLine($"IsArea: {ra.IsArea}");
Console.WriteLine($"SheetName: {ra.SheetName}");
if (ra.IsArea)
{
Console.WriteLine($"Range: {CellsHelper.CellIndexToName(ra.StartRow, ra.StartColumn)}" +
$":{CellsHelper.CellIndexToName(ra.EndRow, ra.EndColumn)}");
}
else
{
Console.WriteLine($"Cell: {CellsHelper.CellIndexToName(ra.StartRow, ra.StartColumn)}");
}
Console.WriteLine();
}
}
}
}
```
### See Also
* class [ReferredArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
