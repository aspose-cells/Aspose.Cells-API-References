##DataLabels.ShowSeriesName
DataLabels property. Indicates whether the series name displays for the data labels on a chart. True to show the series name. False to hide
## DataLabels.ShowSeriesName property
Indicates whether the series name displays for the data labels on a chart. True to show the series name. False to hide.
```csharp
public bool ShowSeriesName { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class DataLabelsPropertyShowSeriesNameDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for chart
worksheet.Cells["A1"].PutValue("Series 1");
worksheet.Cells["A2"].PutValue(10);
worksheet.Cells["A3"].PutValue(20);
worksheet.Cells["A4"].PutValue(30);
worksheet.Cells["B1"].PutValue("Series 2");
worksheet.Cells["B2"].PutValue(15);
worksheet.Cells["B3"].PutValue(25);
worksheet.Cells["B4"].PutValue(35);
// Add a column chart
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
Chart chart = worksheet.Charts[chartIndex];
// Set chart data range
chart.NSeries.Add("A1:A4", true);
chart.NSeries.Add("B1:B4", true);
// Enable data labels for first series
Series series = chart.NSeries[0];
series.DataLabels.ShowValue = true;
// Enable showing series name for specific point's data label
var points = series.Points;
points[1].DataLabels.ShowSeriesName = true;
// Calculate chart
chart.Calculate();
// Save the workbook
workbook.Save("DataLabelsShowSeriesNameDemo.xlsx");
}
}
}
```
### See Also
* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
