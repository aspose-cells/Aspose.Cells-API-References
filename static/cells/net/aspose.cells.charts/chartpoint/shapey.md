##ChartPoint.ShapeY
ChartPoint property. Gets the y coordinate of the upper left corner in units of 1/4000 of charts height after calls Chart.Calculate method
## ChartPoint.ShapeY property
Gets the y coordinate of the upper left corner in units of 1/4000 of chart's height after calls Chart.Calculate() method.
```csharp
public int ShapeY { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using System;
public class ChartPointPropertyShapeYDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for the chart
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["A2"].PutValue("A");
worksheet.Cells["A3"].PutValue("B");
worksheet.Cells["A4"].PutValue("C");
worksheet.Cells["B1"].PutValue("Value");
worksheet.Cells["B2"].PutValue(10);
worksheet.Cells["B3"].PutValue(20);
worksheet.Cells["B4"].PutValue(30);
// Add a column chart
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
Chart chart = worksheet.Charts[chartIndex];
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
// Calculate chart to get shape positions
chart.Calculate();
// Get the first point in the first series
ChartPoint point = chart.NSeries[0].Points[0];
// Display the current ShapeY value (1/4000 of chart's height)
Console.WriteLine("Current ShapeY value: " + point.ShapeY);
// Note: ShapeY is read-only, so we can't set it directly
// To change the position, we would need to modify the underlying data or chart properties
// Demonstrate how ShapeY relates to actual position
Console.WriteLine("ShapeY in pixels: " + point.ShapeYPx);
Console.WriteLine("Chart height in pixels: " + (point.ShapeYPx * 4000 / point.ShapeY));
// Save the result
workbook.Save("ChartPointPropertyShapeYDemo.xlsx");
}
}
}
```
### See Also
* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
