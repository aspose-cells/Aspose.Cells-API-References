##Trendline.Period
Trendline property. Returns or sets the period for the movingaverage trendline
## Trendline.Period property
Returns or sets the period for the moving-average trendline.
```csharp
public int Period { get; set; }
```
### Remarks
This value should be between 2 and 255. And it must be less than the number of the chart points in the series
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class TrendlinePropertyPeriodDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("X");
worksheet.Cells["B1"].PutValue("Y");
for (int i = 2; i <= 10; i++)
{
worksheet.Cells["A" + i].PutValue(i);
worksheet.Cells["B" + i].PutValue(i * 2);
}
// Add a chart
int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 20, 8);
Chart chart = worksheet.Charts[chartIndex];
// Add series
chart.NSeries.Add("B2:B10", true);
chart.NSeries.CategoryData = "A2:A10";
// Add a moving average trendline
int trendlineIndex = chart.NSeries[0].TrendLines.Add(TrendlineType.MovingAverage);
Trendline trendline = chart.NSeries[0].TrendLines[trendlineIndex];
trendline.Period = 3; // Set period for moving average
trendline.Name = "3-Period Moving Average";
// Save the workbook
workbook.Save("TrendlinePeriodDemo.xlsx");
}
}
}
```
### See Also
* class [Trendline](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
