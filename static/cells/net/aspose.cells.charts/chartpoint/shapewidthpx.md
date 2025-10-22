##ChartPoint.ShapeWidthPx
ChartPoint property. Gets the width in units of pixels after calls Chart.Calculate method
## ChartPoint.ShapeWidthPx property
Gets the width in units of pixels after calls Chart.Calculate() method.
```csharp
public int ShapeWidthPx { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using System;
public class ChartPointPropertyShapeWidthPxDemo
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
// Add a column chart
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
Chart chart = worksheet.Charts[chartIndex];
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
// Calculate chart to ensure shape properties are available
chart.Calculate();
// Get the first chart point from first series
ChartPoint point = chart.NSeries[0].Points[0];
// Display the current width of the chart point shape in pixels
Console.WriteLine("Current ShapeWidthPx value: " + point.ShapeWidthPx);
// Note: ShapeWidthPx is read-only, so we can't set it directly
// To change the width, we need to modify the chart's size or other properties
// that would affect the point's width during the next Calculate()
// Change the chart's width to demonstrate how it affects ShapeWidthPx
chart.ChartObject.Width = 1000;
chart.Calculate();
// Display the new width after chart resize
Console.WriteLine("New ShapeWidthPx value after chart resize: " + point.ShapeWidthPx);
// Save the result
workbook.Save("ChartPointPropertyShapeWidthPxDemo.xlsx");
}
}
}
```
### See Also
* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
