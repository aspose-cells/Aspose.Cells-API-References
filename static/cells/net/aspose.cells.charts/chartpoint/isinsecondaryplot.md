##ChartPoint.IsInSecondaryPlot
ChartPoint property. Gets or sets a value indicates whether this data points is in the second pie or bar on a pie of pie or bar of pie chart
## ChartPoint.IsInSecondaryPlot property
Gets or sets a value indicates whether this data points is in the second pie or bar on a pie of pie or bar of pie chart
```csharp
public bool IsInSecondaryPlot { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class ChartPointPropertyIsInSecondaryPlotDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue(50);
worksheet.Cells["A2"].PutValue(100);
worksheet.Cells["A3"].PutValue(150);
worksheet.Cells["B1"].PutValue(60);
worksheet.Cells["B2"].PutValue(32);
worksheet.Cells["B3"].PutValue(50);
// Create pie chart that supports secondary plots
int chartIndex = worksheet.Charts.Add(ChartType.Pie, 5, 0, 25, 10);
Chart chart = worksheet.Charts[chartIndex];
chart.NSeries.Add("A1:B3", true);
// Configure secondary plot
chart.NSeries[0].Points[2].IsInSecondaryPlot = true;
chart.NSeries[0].Points[3].IsInSecondaryPlot = true;
// Save the output
workbook.Save("PieChartWithSecondaryPlot.xlsx");
}
}
}
```
### See Also
* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
