##ChartPoint.GetTopPointCount
ChartPoint method. Gets the number of top points after calls Chart.Calculate method
## ChartPoint.GetTopPointCount method
Gets the number of top points after calls Chart.Calculate() method.
```csharp
public int GetTopPointCount()
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using System;
public class ChartPointMethodGetTopPointCountDemo
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
// Calculate chart to ensure all properties are set
chart.Calculate();
try
{
// Get the first point in the first series
ChartPoint point = chart.NSeries[0].Points[0];
// Call GetTopPointCount method
int topPointCount = point.GetTopPointCount();
// Display the result
Console.WriteLine($"Number of top points: {topPointCount}");
// Demonstrate getting top point coordinates
if (topPointCount > 0)
{
for (int i = 0; i < topPointCount; i++)
{
float x = point.GetTopPointXPx(i);
float y = point.GetTopPointYPx(i);
Console.WriteLine($"Top point {i + 1} coordinates: ({x}, {y})");
}
}
}
catch (Exception ex)
{
Console.WriteLine($"Error executing GetTopPointCount method: {ex.Message}");
}
// Save the result
workbook.Save("MethodGetTopPointCountDemo.xlsx");
}
}
}
```
### See Also
* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
