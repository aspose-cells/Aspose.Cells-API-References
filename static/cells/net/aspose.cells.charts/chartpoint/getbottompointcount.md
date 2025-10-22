##ChartPoint.GetBottomPointCount
ChartPoint method. Gets the number of bottom points after calls Chart.Calculate method
## ChartPoint.GetBottomPointCount method
Gets the number of bottom points after calls Chart.Calculate() method.
```csharp
public int GetBottomPointCount()
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using System;
public class ChartPointMethodGetBottomPointCountDemo
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
// Set chart data range
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
// Calculate chart to ensure all points are calculated
chart.Calculate();
try
{
// Get the first point in the first series
ChartPoint point = chart.NSeries[0].Points[0];
// Call GetBottomPointCount method
int bottomPointCount = point.GetBottomPointCount();
// Display the result
Console.WriteLine($"Number of bottom points: {bottomPointCount}");
// Show coordinates of bottom points
for (int i = 0; i < bottomPointCount; i++)
{
float x = point.GetBottomPointXPx(i);
float y = point.GetBottomPointYPx(i);
Console.WriteLine($"Bottom point {i}: X={x}, Y={y}");
}
}
catch (Exception ex)
{
Console.WriteLine($"Error executing GetBottomPointCount method: {ex.Message}");
}
// Save the result
workbook.Save("MethodGetBottomPointCountDemo.xlsx");
}
}
}
```
### See Also
* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
