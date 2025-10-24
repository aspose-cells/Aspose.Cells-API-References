##SeriesLayoutProperties.ShowMeanMarker
SeriesLayoutProperties property. Indicates whether showing markers denoting the mean
## SeriesLayoutProperties.ShowMeanMarker property
Indicates whether showing markers denoting the mean.
```csharp
public bool ShowMeanMarker { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class SeriesLayoutPropertiesPropertyShowMeanMarkerDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue(10);
worksheet.Cells["A2"].PutValue(20);
worksheet.Cells["A3"].PutValue(30);
worksheet.Cells["A4"].PutValue(40);
// Create chart (using Column chart type which supports mean markers)
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
Chart chart = worksheet.Charts[chartIndex];
// Add series
chart.NSeries.Add("A1:A4", true);
Series series = chart.NSeries[0];
// Configure layout properties with ShowMeanMarker
SeriesLayoutProperties layoutProperties = series.LayoutProperties;
layoutProperties.ShowMeanMarker = true;
layoutProperties.ShowMeanLine = true;
// Save output
workbook.Save("ColumnChartWithMeanMarker.xlsx");
}
}
}
```
### See Also
* class [SeriesLayoutProperties](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
