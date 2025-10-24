##Series.Marker
Series property. Gets the marker
## Series.Marker property
Gets the `marker`.
```csharp
public Marker Marker { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using System.Drawing;
namespace AsposeCellsExamples
{
public class SeriesPropertyMarkerDemo
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
int chartIndex = worksheet.Charts.Add(ChartType.LineWithDataMarkers, 5, 0, 20, 10);
Chart chart = worksheet.Charts[chartIndex];
chart.NSeries.Add("A1:A3", true);
// Customize marker properties
foreach (Series series in chart.NSeries)
{
series.Marker.MarkerStyle = ChartMarkerType.SquarePlus;
series.Marker.MarkerSize = 12;
series.Marker.Border.Color = Color.Red;
series.Marker.BackgroundColor = Color.Yellow;
}
workbook.Save("SeriesMarkerDemo.xlsx");
}
}
}
```
### See Also
* class [Marker](../../marker/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
