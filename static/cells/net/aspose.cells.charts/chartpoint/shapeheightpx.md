##ChartPoint.ShapeHeightPx
ChartPoint property. Gets the height in units of pixels after calls Chart.Calculate method
## ChartPoint.ShapeHeightPx property
Gets the height in units of pixels after calls Chart.Calculate() method.
```csharp
public int ShapeHeightPx { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using System;
public class ChartPointPropertyShapeHeightPxDemo
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
// Calculate the chart to get shape dimensions
chart.Calculate();
// Get the first chart point from the first series
ChartPoint chartPoint = chart.NSeries[0].Points[0];
// Display the current height of the chart point shape in pixels
Console.WriteLine("Current ShapeHeightPx value: " + chartPoint.ShapeHeightPx);
// Note: ShapeHeightPx is read-only, so we can't set it directly
// To change the height, we would need to modify the chart size or data values
// and recalculate the chart
// Change the data value which will affect the chart point size
worksheet.Cells["B2"].PutValue(50);
chart.Calculate();
// Display the new height after changing the data
Console.WriteLine("New ShapeHeightPx value after data change: " + chartPoint.ShapeHeightPx);
// Save the workbook
workbook.Save("ChartPointShapeHeightPxDemo.xlsx");
}
}
}
```
### See Also
* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
