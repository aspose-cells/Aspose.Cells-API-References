##ChartPoint.GetOnCategoryAxisPointYPx
ChartPoint method. Gets ycoordinate of the point on category axis after calls Chart.Calculate method. Only applies to Area chart
## ChartPoint.GetOnCategoryAxisPointYPx method
Gets y-coordinate of the point on category axis after calls Chart.Calculate() method. Only applies to Area chart.
```csharp
public float GetOnCategoryAxisPointYPx(int index)
```
### Remarks
Area 2D chart: index is 0. Area 3D chart: index is 0 or 1.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using System;
public class ChartPointMethodGetOnCategoryAxisPointYPxWithInt32Demo
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
// Add a chart
int chartIndex = worksheet.Charts.Add(ChartType.Area, 5, 0, 20, 10);
Chart chart = worksheet.Charts[chartIndex];
// Set chart data source
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
// Calculate chart to ensure all position properties are calculated
chart.Calculate();
// Get the first chart point from first series
ChartPoint point = chart.NSeries[0].Points[0];
try
{
// Call GetOnCategoryAxisPointYPx with index 0
float yPx = point.GetOnCategoryAxisPointYPx(0);
// Display the result
Console.WriteLine($"Y coordinate of point on category axis: {yPx} pixels");
// Save the workbook
workbook.Save("ChartPointGetOnCategoryAxisPointYPxDemo.xlsx");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing GetOnCategoryAxisPointYPx method: {ex.Message}");
}
}
}
}
```
### See Also
* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
