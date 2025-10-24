##Series.HasRadarAxisLabels
Series property. True if a radar chart has category axis labels. Applies only to radar charts
## Series.HasRadarAxisLabels property
True if a radar chart has category axis labels. Applies only to radar charts.
```csharp
public bool HasRadarAxisLabels { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class SeriesPropertyHasRadarAxisLabelsDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for radar chart
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["A2"].PutValue("Cat1");
worksheet.Cells["A3"].PutValue("Cat2");
worksheet.Cells["A4"].PutValue("Cat3");
worksheet.Cells["B1"].PutValue("Series1");
worksheet.Cells["B2"].PutValue(4);
worksheet.Cells["B3"].PutValue(2);
worksheet.Cells["B4"].PutValue(5);
// Add a radar chart
int chartIndex = worksheet.Charts.Add(ChartType.Radar, 5, 0, 20, 8);
Chart chart = worksheet.Charts[chartIndex];
// Add series data
int seriesIndex = chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
// Get the series and set radar axis labels
Series series = chart.NSeries[seriesIndex];
series.HasRadarAxisLabels = true; // This is the key property being demonstrated
// Save the workbook
workbook.Save("RadarChartWithAxisLabels.xlsx");
}
}
}
```
### See Also
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
