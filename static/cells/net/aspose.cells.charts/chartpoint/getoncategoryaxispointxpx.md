##ChartPoint.GetOnCategoryAxisPointXPx
ChartPoint method. Gets xcoordinate of the point on category axis after calls Chart.Calculate method. Only applies to Area chart
## ChartPoint.GetOnCategoryAxisPointXPx method
Gets x-coordinate of the point on category axis after calls Chart.Calculate() method. Only applies to Area chart.
```csharp
public float GetOnCategoryAxisPointXPx(int index)
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
public class ChartPointMethodGetOnCategoryAxisPointXPxWithInt32Demo
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
int chartIndex = worksheet.Charts.Add(ChartType.Area, 5, 0, 20, 8);
Chart chart = worksheet.Charts[chartIndex];
// Set chart data source
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
// Calculate chart
chart.Calculate();
try
{
// Get the first chart point
ChartPoint point = chart.NSeries[0].Points[0];
// Call GetOnCategoryAxisPointXPx with index 0
float xPosition = point.GetOnCategoryAxisPointXPx(0);
// Display the result
Console.WriteLine($"X position of first category axis point: {xPosition} pixels");
// Save the workbook
workbook.Save("ChartPointGetOnCategoryAxisPointXPxDemo.xlsx");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing GetOnCategoryAxisPointXPx method: {ex.Message}");
}
}
}
}
```
### See Also
* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
