##Series.FirstSliceAngle
Series property. Gets or sets the angle of the first piechart or doughnutchart slice in degrees clockwise from vertical. Applies only to pie 3D pie and doughnut charts 0 to 360
## Series.FirstSliceAngle property
Gets or sets the angle of the first pie-chart or doughnut-chart slice, in degrees (clockwise from vertical). Applies only to pie, 3-D pie, and doughnut charts, 0 to 360.
```csharp
public short FirstSliceAngle { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class SeriesPropertyFirstSliceAngleDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for pie chart
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["A2"].PutValue("Apple");
worksheet.Cells["A3"].PutValue("Orange");
worksheet.Cells["A4"].PutValue("Banana");
worksheet.Cells["B1"].PutValue("Value");
worksheet.Cells["B2"].PutValue(50);
worksheet.Cells["B3"].PutValue(30);
worksheet.Cells["B4"].PutValue(20);
// Add pie chart
int chartIndex = worksheet.Charts.Add(ChartType.Pie, 5, 0, 15, 5);
Chart chart = worksheet.Charts[chartIndex];
// Set chart data range
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
// Get the first series and set FirstSliceAngle
Series series = chart.NSeries[0];
series.FirstSliceAngle = 45; // Rotate pie chart by 45 degrees
workbook.Save("PieChartWithFirstSliceAngle.xlsx");
}
}
}
```
### See Also
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
