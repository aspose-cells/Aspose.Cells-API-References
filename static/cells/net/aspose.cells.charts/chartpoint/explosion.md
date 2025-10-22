##ChartPoint.Explosion
ChartPoint property. The distance of an open pie slice from the center of the pie chart is expressed as a percentage of the pie diameter
## ChartPoint.Explosion property
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
public class ChartPointPropertyExplosionDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for chart
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["A2"].PutValue("A");
worksheet.Cells["A3"].PutValue("B");
worksheet.Cells["A4"].PutValue("C");
worksheet.Cells["B1"].PutValue("Value");
worksheet.Cells["B2"].PutValue(10);
worksheet.Cells["B3"].PutValue(20);
worksheet.Cells["B4"].PutValue(30);
// Add a pie chart
int chartIndex = worksheet.Charts.Add(ChartType.Pie, 5, 0, 20, 8);
Chart chart = worksheet.Charts[chartIndex];
// Set chart data range
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
// Access the first chart point and set explosion
ChartPoint point = chart.NSeries[0].Points[0];
point.Explosion = 15; // Set explosion distance (15 points)
// Save the workbook
workbook.Save("ChartPointExplosionDemo.xlsx");
}
}
}
```
### See Also
* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
