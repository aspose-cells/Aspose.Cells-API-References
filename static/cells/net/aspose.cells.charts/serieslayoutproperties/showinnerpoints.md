##SeriesLayoutProperties.ShowInnerPoints
SeriesLayoutProperties property. Indicates whether showing nonoutlier data points
## SeriesLayoutProperties.ShowInnerPoints property
Indicates whether showing non-outlier data points.
```csharp
public bool ShowInnerPoints { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class SeriesLayoutPropertiesPropertyShowInnerPointsDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for box and whisker chart
worksheet.Cells["A1"].PutValue("Series 1");
worksheet.Cells["A2"].PutValue(10);
worksheet.Cells["A3"].PutValue(40);
worksheet.Cells["A4"].PutValue(15);
worksheet.Cells["A5"].PutValue(20);
worksheet.Cells["A6"].PutValue(25);
worksheet.Cells["A7"].PutValue(30);
worksheet.Cells["A8"].PutValue(35);
worksheet.Cells["A9"].PutValue(40);
worksheet.Cells["A10"].PutValue(45);
worksheet.Cells["A11"].PutValue(50);
// Add a box and whisker chart
int chartIndex = worksheet.Charts.Add(ChartType.BoxWhisker, 5, 0, 20, 8);
Chart chart = worksheet.Charts[chartIndex];
// Add series to the chart
chart.NSeries.Add("A2:A11", true);
Series series = chart.NSeries[0];
// Set series layout properties
SeriesLayoutProperties layout = series.LayoutProperties;
layout.ShowInnerPoints = true; // Demonstrate ShowInnerPoints property
layout.ShowOutlierPoints = true;
layout.ShowMeanMarker = true;
// Calculate chart
chart.Calculate();
// Save the workbook
workbook.Save("BoxWhiskerChart_ShowInnerPoints.xlsx");
}
}
}
```
### See Also
* class [SeriesLayoutProperties](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
