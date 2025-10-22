##Chart.Move
Chart method. Moves the chart to a specified location
## Chart.Move method
Moves the chart to a specified location.
```csharp
public void Move(int upperLeftRow, int upperLeftColumn, int lowerRightRow, int lowerRightColumn)
```
| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftColumn | Int32 | Upper left column index. |
| upperLeftRow | Int32 | Upper left row index. |
| lowerRightColumn | Int32 | Lower right column index |
| lowerRightRow | Int32 | Lower right row index |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using System;
public class ChartMethodMoveWithInt32Int32Int32Int32Demo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for the chart
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["A2"].PutValue("Fruits");
worksheet.Cells["A3"].PutValue("Vegetables");
worksheet.Cells["B1"].PutValue("Value");
worksheet.Cells["B2"].PutValue(50);
worksheet.Cells["B3"].PutValue(30);
// Add a chart to the worksheet
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
Chart chart = worksheet.Charts[chartIndex];
// Set chart data source
chart.NSeries.Add("B2:B3", true);
chart.NSeries.CategoryData = "A2:A3";
try
{
// Original chart position
Console.WriteLine($"Original position - UpperLeftRow: {chart.ChartObject.UpperLeftRow}, UpperLeftColumn: {chart.ChartObject.UpperLeftColumn}");
// Move the chart to new position (rows 10-20, columns 2-8)
chart.Move(10, 2, 20, 8);
// Display new position
Console.WriteLine($"New position - UpperLeftRow: {chart.ChartObject.UpperLeftRow}, UpperLeftColumn: {chart.ChartObject.UpperLeftColumn}");
// Save the workbook
workbook.Save("ChartMoveDemo.xlsx");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing Move method: {ex.Message}");
}
}
}
}
```
### See Also
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
