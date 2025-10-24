##ChartPoint.ShapeX
ChartPoint property. Gets the x coordinate of the upper left corner in units of 1/4000 of charts width after calls Chart.Calculate method
## ChartPoint.ShapeX property
Gets the x coordinate of the upper left corner in units of 1/4000 of chart's width after calls Chart.Calculate() method.
```csharp
public int ShapeX { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using System;
public class ChartPointPropertyShapeXDemo
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
// Set chart data range
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
// Calculate chart to ensure ShapeX is populated
chart.Calculate();
// Get the first point in the first series
ChartPoint point = chart.NSeries[0].Points[0];
// Display the ShapeX value (1/4000 of chart's width)
Console.WriteLine("ShapeX value (1/4000 units): " + point.ShapeX);
Console.WriteLine("ShapeX value (pixels): " + point.ShapeXPx);
// Demonstrate using ShapeX to position elements relative to the chart point
// Note: Since ShapeX is read-only, we can't modify it directly,
// but we can use it to position other elements
if (point.ShapeX > 0)
{
// Add a text box aligned with the chart point's X position
Aspose.Cells.Drawing.TextBox textBox = worksheet.Shapes.AddTextBox(
point.ShapeXPx, 100, 100, 50, 100, 50);
textBox.Text = "Point 1";
}
// Save the result
workbook.Save("ChartPointShapeXDemo.xlsx");
}
}
}
```
### See Also
* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
