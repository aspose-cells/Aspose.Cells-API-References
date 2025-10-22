##Chart.GetChartDataRange
Chart method. Gets the data source range of the chart
## Chart.GetChartDataRange method
Gets the data source range of the chart.
```csharp
public string GetChartDataRange()
```
### Return Value
The data source.
### Remarks
Only supports range.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class ChartMethodGetChartDataRangeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for chart
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["B1"].PutValue("Series1");
worksheet.Cells["C1"].PutValue("Series2");
worksheet.Cells["A2"].PutValue("A");
worksheet.Cells["B2"].PutValue(10);
worksheet.Cells["C2"].PutValue(20);
worksheet.Cells["A3"].PutValue("B");
worksheet.Cells["B3"].PutValue(30);
worksheet.Cells["C3"].PutValue(40);
worksheet.Cells["A4"].PutValue("C");
worksheet.Cells["B4"].PutValue(50);
worksheet.Cells["C4"].PutValue(60);
// Add a chart to the worksheet
int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 8);
Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
// Set chart data range
chart.NSeries.Add("=Sheet1!$B$1:$C$4", true);
// Get and display the chart data range
string dataRange = chart.GetChartDataRange();
Console.WriteLine("Chart Data Range: " + dataRange);
// Save the workbook
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
