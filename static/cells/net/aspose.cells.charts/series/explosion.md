##Series.Explosion
Series property. The distance of an open pie slice from the center of the pie chart is expressed as a percentage of the pie diameter
## Series.Explosion property
The distance of an open pie slice from the center of the pie chart is expressed as a percentage of the pie diameter.
```csharp
public int Explosion { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class SeriesPropertyExplosionDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Category 1");
worksheet.Cells["A2"].PutValue("Category 2");
worksheet.Cells["A3"].PutValue("Category 3");
worksheet.Cells["B1"].PutValue(10);
worksheet.Cells["B2"].PutValue(20);
worksheet.Cells["B3"].PutValue(30);
// Add pie chart
int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Pie, 5, 0, 15, 5);
Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
// Add series
int seriesIndex = chart.NSeries.Add("B1:B3", true);
chart.NSeries.CategoryData = "A1:A3";
// Access series and set explosion
Aspose.Cells.Charts.Series series = chart.NSeries[seriesIndex];
series.Explosion = 15; // Set explosion value (0-100)
workbook.Save("PieChartExplosionDemo.xlsx");
}
}
}
```
### See Also
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
