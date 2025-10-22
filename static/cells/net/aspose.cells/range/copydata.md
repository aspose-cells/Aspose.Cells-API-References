##Range.CopyData
Range method. Copies cell data including formulas from a source range
## Range.CopyData method
Copies cell data (including formulas) from a source range.
```csharp
public void CopyData(Range range)
```
| Parameter | Type | Description |
| --- | --- | --- |
| range | Range | Source [`Range`](../) object. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class RangeMethodCopyDataWithRangeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Get the first worksheet and add some data
Worksheet sheetSrc = workbook.Worksheets[0];
sheetSrc.Name = "Source";
sheetSrc.Cells["A1"].PutValue("Source Data");
sheetSrc.Cells["B1"].PutValue(100);
sheetSrc.Cells["A2"].PutValue("More Data");
sheetSrc.Cells["B2"].PutValue(200);
// Add a destination worksheet
Worksheet sheetDest = workbook.Worksheets[workbook.Worksheets.Add()];
sheetDest.Name = "Destination";
// Create source and destination ranges
Aspose.Cells.Range rangeSrc = sheetSrc.Cells.CreateRange("A1:B2");
Aspose.Cells.Range rangeDest = sheetDest.Cells.CreateRange("C3:D4");
// Copy data from source range to destination range
rangeDest.CopyData(rangeSrc);
// Save the workbook
workbook.Save("RangeCopyDataDemo.xlsx");
}
}
}
```
### See Also
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
