##Series.TrendLines
Series property. Returns all the trendlines of this series
## Series.TrendLines property
Returns all the trendlines of this series.
```csharp
public TrendlineCollection TrendLines { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class SeriesPropertyTrendLinesDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add sample data
sheet.Cells["A1"].PutValue("X");
sheet.Cells["A2"].PutValue(1);
sheet.Cells["A3"].PutValue(2);
sheet.Cells["A4"].PutValue(3);
sheet.Cells["A5"].PutValue(4);
sheet.Cells["B1"].PutValue("Y");
sheet.Cells["B2"].PutValue(2);
sheet.Cells["B3"].PutValue(4);
sheet.Cells["B4"].PutValue(8);
sheet.Cells["B5"].PutValue(16);
// Add a chart
int chartIndex = sheet.Charts.Add(ChartType.Line, 5, 0, 20, 8);
Chart chart = sheet.Charts[chartIndex];
// Set chart data source
chart.NSeries.Add("B2:B5", true);
chart.NSeries.CategoryData = "A2:A5";
// Add exponential trendline to the first series and get it by index
int trendlineIndex = chart.NSeries[0].TrendLines.Add(TrendlineType.Exponential);
Trendline trendline = chart.NSeries[0].TrendLines[trendlineIndex];
trendline.DisplayEquation = true;
trendline.DisplayRSquared = true;
// Save the workbook
workbook.Save("TrendLinesDemo.xlsx");
}
}
}
```
### See Also
* class [TrendlineCollection](../../trendlinecollection/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
