##SparklineGroupCollection.Item
SparklineGroupCollection property. Gets the SparklineGroup element at the specified index
## SparklineGroupCollection indexer
Gets the [`SparklineGroup`](../../sparklinegroup/) element at the specified index.
```csharp
public SparklineGroup this[int index] { get; }
```
| Parameter | Description |
| --- | --- |
| index | The zero based index of the element. |
### Return Value
The element at the specified index.
### Examples
```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class SparklineGroupCollectionPropertyItemDemo
{
public static void Run()
{
Workbook wb = new Workbook();
Worksheet ws = wb.Worksheets[0];
// Add sample data
ws.Cells["A1"].PutValue(5);
ws.Cells["A2"].PutValue(3);
ws.Cells["A3"].PutValue(7);
ws.Cells["A4"].PutValue(2);
ws.Cells["A5"].PutValue(9);
// Define data range and location for sparklines
string dataRange = "'" + ws.Name + "'!A1:A5";
CellArea location = new CellArea();
location.StartRow = 0;
location.EndRow = 0;
location.StartColumn = 1;
location.EndColumn = 1;
// Add sparkline group
int index = ws.SparklineGroups.Add(SparklineType.Line, dataRange, false, location);
// Access the sparkline group using Item property
SparklineGroup group = ws.SparklineGroups[index];
// Customize the sparkline
CellsColor color = wb.CreateCellsColor();
color.Color = Color.Blue;
group.SeriesColor = color;
// Save the workbook
wb.Save("SparklineGroupCollectionPropertyItemDemo.xlsx", SaveFormat.Xlsx);
}
}
}
```
### See Also
* class [SparklineGroup](../../sparklinegroup/)
* class [SparklineGroupCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
