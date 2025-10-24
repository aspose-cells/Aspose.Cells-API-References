##ChartPoint.GetOnCategoryAxisPointCount
ChartPoint method. Gets the number of the points on category axis after calls Chart.Calculate method. Only applies to area chart
## ChartPoint.GetOnCategoryAxisPointCount method
Gets the number of the points on category axis after calls Chart.Calculate() method. Only applies to area chart.
```csharp
public int GetOnCategoryAxisPointCount()
```
### Remarks
Area 2D chart return 1 Area 3D chart return 2.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using System;
public class ChartPointMethodGetOnCategoryAxisPointCountDemo
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
// Add an area chart
int chartIndex = worksheet.Charts.Add(ChartType.Area, 5, 0, 20, 8);
Chart chart = worksheet.Charts[chartIndex];
// Set chart data range
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
// Calculate chart to ensure all chart points are calculated
chart.Calculate();
try
{
// Get the first chart point from first series
ChartPoint point = chart.NSeries[0].Points[0];
// Call GetOnCategoryAxisPointCount method
int pointCount = point.GetOnCategoryAxisPointCount();
Console.WriteLine($"Number of points on category axis: {pointCount}");
// Display coordinates of each point on category axis
for (int i = 0; i < pointCount; i++)
{
float x = point.GetOnCategoryAxisPointXPx(i);
float y = point.GetOnCategoryAxisPointYPx(i);
Console.WriteLine($"Point {i}: X={x}, Y={y}");
}
}
catch (Exception ex)
{
Console.WriteLine($"Error executing GetOnCategoryAxisPointCount method: {ex.Message}");
}
// Save the workbook
workbook.Save("MethodGetOnCategoryAxisPointCountDemo.xlsx");
}
}
}
```
### See Also
* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
