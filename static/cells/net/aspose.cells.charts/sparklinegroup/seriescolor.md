##SparklineGroup.SeriesColor
SparklineGroup property. Gets and sets the color of the sparklines in the sparkline group
## SparklineGroup.SeriesColor property
Gets and sets the color of the sparklines in the sparkline group.
```csharp
public CellsColor SeriesColor { get; set; }
```
### Examples
```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class SparklineGroupPropertySeriesColorDemo
{
public static void Run()
{
Workbook wb = new Workbook();
Worksheet ws = wb.Worksheets[0];
// Sample data
ws.Cells["A1"].PutValue(5);
ws.Cells["A2"].PutValue(8);
ws.Cells["A3"].PutValue(3);
// Create sparkline group
CellArea dataRange = new CellArea { StartRow = 0, EndRow = 2, StartColumn = 0, EndColumn = 0 };
CellArea locationRange = new CellArea { StartRow = 0, EndRow = 0, StartColumn = 1, EndColumn = 1 };
int index = ws.SparklineGroups.Add(SparklineType.Column, "A1:A3", false, locationRange);
// Set series color
SparklineGroup group = ws.SparklineGroups[index];
CellsColor color = wb.CreateCellsColor();
color.Color = Color.Blue;
group.SeriesColor = color;
wb.Save("SparklineSeriesColorDemo.xlsx", SaveFormat.Xlsx);
}
}
}
```
### See Also
* class [CellsColor](../../../aspose.cells/cellscolor/)
* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
