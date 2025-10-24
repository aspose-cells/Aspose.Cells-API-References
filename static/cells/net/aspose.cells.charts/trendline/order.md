##Trendline.Order
Trendline property. Returns or sets the trendline order an integer greater than 1 when the trendline type is Polynomial. The order must be between 2 and 6
## Trendline.Order property
Returns or sets the trendline order (an integer greater than 1) when the trendline type is Polynomial. The order must be between 2 and 6.
```csharp
public int Order { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class TrendlinePropertyOrderDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue(1);
worksheet.Cells["A2"].PutValue(2);
worksheet.Cells["A3"].PutValue(3);
worksheet.Cells["B1"].PutValue(4);
worksheet.Cells["B2"].PutValue(5);
worksheet.Cells["B3"].PutValue(6);
int chartIndex = worksheet.Charts.Add(ChartType.Scatter, 5, 0, 20, 8);
Chart chart = worksheet.Charts[chartIndex];
chart.NSeries.Add("A1:A3", true);
chart.NSeries.CategoryData = "B1:B3";
Series series = chart.NSeries[0];
int trendlineIndex = series.TrendLines.Add(TrendlineType.Polynomial);
Trendline trendline = series.TrendLines[trendlineIndex];
trendline.Order = 3;
workbook.Save("TrendlineOrderDemo.xlsx");
Workbook loadedWorkbook = new Workbook("TrendlineOrderDemo.xlsx");
Chart loadedChart = loadedWorkbook.Worksheets[0].Charts[0];
Trendline loadedTrendline = loadedChart.NSeries[0].TrendLines[0];
Console.WriteLine("Trendline Order: " + loadedTrendline.Order);
}
}
}
```
### See Also
* class [Trendline](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
