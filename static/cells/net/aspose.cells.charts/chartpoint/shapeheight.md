##ChartPoint.ShapeHeight
ChartPoint property. Gets the height in units of 1/4000 of charts height after calls Chart.Calculate method
## ChartPoint.ShapeHeight property
Gets the height in units of 1/4000 of chart's height after calls Chart.Calculate() method.
```csharp
public int ShapeHeight { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using System;
public class ChartPointPropertyShapeHeightDemo
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
// Set chart data source
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
// Calculate chart to ensure shape properties are available
chart.Calculate();
// Get the first point in the first series
ChartPoint point = chart.NSeries[0].Points[0];
// Display the current ShapeHeight value (in 1/4000 of chart's height)
Console.WriteLine("Current ShapeHeight value: " + point.ShapeHeight);
// Note: ShapeHeight is read-only, so we can't set it directly
// To change the height, we need to modify the chart size or other properties
// Demonstrate the effect by changing the chart height
Console.WriteLine("Original chart height: " + chart.ChartObject.Height);
chart.ChartObject.Height = 400;
chart.Calculate(); // Recalculate to update shape properties
// Display the new ShapeHeight value after changing chart height
Console.WriteLine("New ShapeHeight value after chart resize: " + point.ShapeHeight);
// Save the result
workbook.Save("ChartPointPropertyShapeHeightDemo.xlsx");
}
}
}
```
### See Also
* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
