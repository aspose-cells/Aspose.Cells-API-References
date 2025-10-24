##ChartPointCollection.RemoveAt
ChartPointCollection method. Removes point at the index of the series
## ChartPointCollection.RemoveAt method
Removes point at the index of the series..
```csharp
public void RemoveAt(int index)
```
| Parameter | Type | Description |
| --- | --- | --- |
| index | Int32 | The index of the point. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using System;
public class ChartPointCollectionMethodRemoveAtWithInt32Demo
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
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
Chart chart = worksheet.Charts[chartIndex];
// Set chart data range
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
// Get the first series' points collection
ChartPointCollection points = chart.NSeries[0].Points;
try
{
// Display initial count
Console.WriteLine($"Initial points count: {points.Count}");
// Remove the point at index 1 (second point)
points.RemoveAt(1);
// Display result
Console.WriteLine($"Points count after RemoveAt: {points.Count}");
Console.WriteLine("Point at index 1 removed successfully.");
// Save the workbook
workbook.Save("ChartPointCollectionRemoveAtDemo.xlsx");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing RemoveAt method: {ex.Message}");
}
}
}
}
```
### See Also
* class [ChartPointCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
