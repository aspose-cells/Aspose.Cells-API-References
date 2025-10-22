##Chart.IsChartDataChanged
Chart method. Detects if a charts data source has changed
## Chart.IsChartDataChanged method
Detects if a chart's data source has changed.
```csharp
public bool IsChartDataChanged()
```
### Return Value
Returns true if the chart has changed otherwise returns false
### Remarks
The method detects the changes in the chart's data source before rendering the chart to image format. At first Chart.toImage call, the chart source data (e.g. XValuesParseData, ValuesParseData) will be recorded. Before calling the Chart.toImage method again, call IsChartDataChanged method to check if Chart needs re-rendering.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using System;
public class ChartMethodIsChartDataChangedDemo
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
// Add a chart to the worksheet
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
Chart chart = worksheet.Charts[chartIndex];
// Set chart data range
chart.SetChartDataRange("A1:B4", true);
try
{
// Check if chart data has changed (should be false initially)
bool isChanged = chart.IsChartDataChanged();
Console.WriteLine($"Chart data changed after creation: {isChanged}");
// Modify the chart data
worksheet.Cells["B2"].PutValue(15);
// Check again if chart data has changed
isChanged = chart.IsChartDataChanged();
Console.WriteLine($"Chart data changed after modification: {isChanged}");
// Calculate the chart to update it
chart.Calculate();
// Check after calculation
isChanged = chart.IsChartDataChanged();
Console.WriteLine($"Chart data changed after calculation: {isChanged}");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing IsChartDataChanged method: {ex.Message}");
}
// Save the result
workbook.Save("ChartMethodIsChartDataChangedDemo.xlsx");
}
}
}
```
### See Also
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
