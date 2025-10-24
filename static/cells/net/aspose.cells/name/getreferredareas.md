##Name.GetReferredAreas
Name method. Gets all references referred by this name
## Name.GetReferredAreas method
Gets all references referred by this name.
```csharp
public ReferredArea[] GetReferredAreas(bool recalculate)
```
| Parameter | Type | Description |
| --- | --- | --- |
| recalculate | Boolean | whether recalculate it if this name has been calculated before this invocation. |
### Return Value
All ranges.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class NameMethodGetReferredAreasWithBooleanDemo
{
public static void Run()
{
// Create a workbook
Workbook wb = new Workbook();
// Add some data to worksheet
wb.Worksheets[0].Cells[3, 3].PutValue("v03");
// Create a named range with multiple references
Name n = wb.Worksheets.Names[wb.Worksheets.Names.Add("testname")];
n.RefersTo = "='C:\\[extlink1.xlsx]Sheet1'!$A$1:$B$2,'C:\\[extlink2.xlsx]Sheet2'!$C$3,Sheet1!$D$4,'C:\\[extlink1.xlsx]Sheet1'!E5";
// Get referred areas with external links
ReferredArea[] ras = n.GetReferredAreas(true);
// Display information about each referred area
Console.WriteLine("Number of referred areas: " + ras.Length);
for (int i = 0; i < ras.Length; i++)
{
ReferredArea ra = ras[i];
Console.WriteLine($"\nArea {i + 1}:");
Console.WriteLine($"IsExternalLink: {ra.IsExternalLink}");
if (ra.IsExternalLink)
{
Console.WriteLine($"ExternalFileName: {ra.ExternalFileName}");
}
Console.WriteLine($"SheetName: {ra.SheetName}");
Console.WriteLine($"IsArea: {ra.IsArea}");
if (ra.IsArea)
{
Console.WriteLine($"Range: {CellsHelper.CellIndexToName(ra.StartRow, ra.StartColumn)}" +
$" to {CellsHelper.CellIndexToName(ra.EndRow, ra.EndColumn)}");
}
else
{
Console.WriteLine($"Cell: {CellsHelper.CellIndexToName(ra.StartRow, ra.StartColumn)}");
}
}
// Create external workbook and update values
Workbook wb1 = new Workbook();
wb1.Worksheets[0].Cells[0, 0].PutValue("v10");
wb1.Worksheets[0].Cells[1, 1].PutValue("v11");
wb1.Worksheets[0].Cells[4, 4].PutValue("v14");
// Update linked data source
wb.UpdateLinkedDataSource(new Workbook[]{wb1});
// Display some values from referred areas
Console.WriteLine("\nValues from referred areas:");
Console.WriteLine($"Area1[0,0]: {ras[0].GetValue(0, 0)}");
Console.WriteLine($"Area1[1,1]: {ras[0].GetValue(1, 1)}");
Console.WriteLine($"Area3[0,0]: {ras[2].GetValue(0, 0)}");
Console.WriteLine($"Area4[0,0]: {ras[3].GetValue(0, 0)}");
}
}
}
```
### See Also
* class [ReferredArea](../../referredarea/)
* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
