##SparklineCollection.Item
SparklineCollection property. Gets the Sparkline element at the specified index
## SparklineCollection indexer
Gets the [`Sparkline`](../../sparkline/) element at the specified index.
```csharp
public Sparkline this[int index] { get; }
```
| Parameter | Description |
| --- | --- |
| index | The zero based index of the element. |
### Return Value
The element at the specified index.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class SparklineCollectionPropertyItemDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue(5);
worksheet.Cells["B1"].PutValue(3);
worksheet.Cells["C1"].PutValue(7);
worksheet.Cells["D1"].PutValue(2);
// Create sparkline group
SparklineGroupCollection sparklineGroups = worksheet.SparklineGroups;
int idx = sparklineGroups.Add(SparklineType.Line, "A1:D1", false, CellArea.CreateCellArea(0, 4, 0, 4));
SparklineGroup group = sparklineGroups[idx];
// Access sparklines using Item property
Sparkline sparkline = group.Sparklines[0];
Console.WriteLine("Sparkline Data Range: " + sparkline.DataRange);
Console.WriteLine("Sparkline Type: " + group.Type);
// Modify sparkline data
worksheet.Cells["A1"].PutValue(8);
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [Sparkline](../../sparkline/)
* class [SparklineCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
