##Marker.BackgroundColor
Marker property. Represents the marker background color in a line chart scatter chart or radar chart
## Marker.BackgroundColor property
Represents the marker background color in a line chart, scatter chart, or radar chart.
```csharp
public Color BackgroundColor { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using System.Drawing;
namespace AsposeCellsExamples
{
public class MarkerPropertyBackgroundColorDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue(1);
worksheet.Cells["A2"].PutValue(2);
worksheet.Cells["A3"].PutValue(3);
// Create chart
int chartIndex = worksheet.Charts.Add(ChartType.LineWithDataMarkers, 5, 0, 15, 5);
Chart chart = worksheet.Charts[chartIndex];
chart.NSeries.Add("A1:A3", true);
// Customize marker appearance
foreach (Series series in chart.NSeries)
{
series.Marker.MarkerStyle = ChartMarkerType.Circle;
series.Marker.MarkerSize = 12;
series.Marker.Border.Color = System.Drawing.Color.Blue;
series.Marker.BackgroundColor = System.Drawing.Color.LightGreen; // Demonstrating BackgroundColor property
}
workbook.Save("MarkerBackgroundColorDemo.xlsx");
}
}
}
```
### See Also
* class [Marker](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
