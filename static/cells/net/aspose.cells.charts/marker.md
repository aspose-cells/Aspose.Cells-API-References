##Class Marker
Aspose.Cells.Charts.Marker class. Represents the marker in a line chart scatter chart or radar chart
## Marker class
Represents the marker in a line chart, scatter chart, or radar chart.
```csharp
public class Marker
```
## Properties
| Name | Description |
| --- | --- |
| [Area](../../aspose.cells.charts/marker/area/) { get; } | Gets the [`area`](./area/). |
| [BackgroundColor](../../aspose.cells.charts/marker/backgroundcolor/) { get; set; } | Represents the marker background color in a line chart, scatter chart, or radar chart. |
| [BackgroundColorSetType](../../aspose.cells.charts/marker/backgroundcolorsettype/) { get; set; } | Gets or sets the marker background color set type. |
| [Border](../../aspose.cells.charts/marker/border/) { get; } | Gets the [`border`](../../aspose.cells.drawing/line/). |
| [ForegroundColor](../../aspose.cells.charts/marker/foregroundcolor/) { get; set; } | Represents the marker foreground color in a line chart, scatter chart, or radar chart. |
| [ForegroundColorSetType](../../aspose.cells.charts/marker/foregroundcolorsettype/) { get; set; } | Gets or sets the marker foreground color set type. |
| [MarkerSize](../../aspose.cells.charts/marker/markersize/) { get; set; } | Represents the marker size in unit of points. Applies to line chart, scatter chart, or radar chart. |
| [MarkerSizePx](../../aspose.cells.charts/marker/markersizepx/) { get; set; } | Represents the marker size in unit of pixels. Applies to line chart, scatter chart, or radar chart. |
| [MarkerStyle](../../aspose.cells.charts/marker/markerstyle/) { get; set; } | Represents the marker style. Applies to line chart, scatter chart, or radar chart. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System;
using System.Drawing;
public class MarkerDemo
{
public static void MarkerExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Obtain the reference of the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to cells
worksheet.Cells["A1"].PutValue(50);
worksheet.Cells["A2"].PutValue(100);
worksheet.Cells["A3"].PutValue(150);
worksheet.Cells["B1"].PutValue(60);
worksheet.Cells["B2"].PutValue(32);
worksheet.Cells["B3"].PutValue(50);
// Add a chart to the worksheet
int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 15, 5);
Chart chart = worksheet.Charts[chartIndex];
// Add NSeries (chart data source) to the chart ranging from "A1" cell to "B3"
chart.NSeries.Add("A1:B3", true);
// Access the first series
Series series = chart.NSeries[0];
// Set marker properties
series.Marker.MarkerStyle = ChartMarkerType.Circle;
series.Marker.MarkerSize = 10; // Size in points
series.Marker.MarkerSizePx = 20; // Size in pixels
series.Marker.ForegroundColor = Color.Red;
series.Marker.ForegroundColorSetType = FormattingType.Custom;
series.Marker.BackgroundColor = Color.Yellow;
series.Marker.BackgroundColorSetType = FormattingType.Custom;
// Save the workbook
workbook.Save("MarkerExample.xlsx");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)
