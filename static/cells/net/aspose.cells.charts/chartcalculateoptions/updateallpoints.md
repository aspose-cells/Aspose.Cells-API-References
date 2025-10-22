##ChartCalculateOptions.UpdateAllPoints
ChartCalculateOptions property. Whether update all data points when performing the chart calculation. Default False. When you want to get the value for each data point in the chart specifically set it to true. If this parameter is set to True the new data points may be generated when chart is calculated. This could make the Excel file larger
## ChartCalculateOptions.UpdateAllPoints property
Whether update all data points when performing the chart calculation. Default: False. When you want to get the value for each data point in the chart specifically, set it to true. If this parameter is set to True, the new data points may be generated when chart is calculated. This could make the Excel file larger.
```csharp
public bool UpdateAllPoints { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class ChartCalculateOptionsPropertyUpdateAllPointsDemo
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
worksheet.Cells["B1"].PutValue("Series1");
worksheet.Cells["B2"].PutValue(100);
worksheet.Cells["B3"].PutValue(200);
worksheet.Cells["B4"].PutValue(300);
worksheet.Cells["C1"].PutValue("Series2");
worksheet.Cells["C2"].PutValue(400);
worksheet.Cells["C3"].PutValue(500);
worksheet.Cells["C4"].PutValue(600);
// Add a chart
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
// Set chart data range
chart.NSeries.Add("B2:B4", true);
chart.NSeries.Add("C2:C4", true);
chart.NSeries.CategoryData = "A2:A4";
// Enable data labels
foreach (Aspose.Cells.Charts.Series series in chart.NSeries)
{
series.DataLabels.ShowValue = true;
}
// Calculate chart with UpdateAllPoints option
chart.Calculate(new Aspose.Cells.Charts.ChartCalculateOptions() { UpdateAllPoints = true });
// Output some data label values to demonstrate the result
Console.WriteLine("Series1 Point1 Label: " + chart.NSeries[0].Points[0].DataLabels.Text);
Console.WriteLine("Series2 Point2 Label: " + chart.NSeries[1].Points[1].DataLabels.Text);
}
}
}
```
### See Also
* class [ChartCalculateOptions](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
