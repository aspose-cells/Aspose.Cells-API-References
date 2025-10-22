##Trendline.Backward
Trendline property. Returns or sets the number of periods or units on a scatter chart that the trendline extends backward. The number of periods must be greater than or equal to zero. If the chart type is column the number of periods must be between 0 and 0.5
## Trendline.Backward property
Returns or sets the number of periods (or units on a scatter chart) that the trendline extends backward. The number of periods must be greater than or equal to zero. If the chart type is column ,the number of periods must be between 0 and 0.5
```csharp
public double Backward { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class TrendlinePropertyBackwardDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue(50);
worksheet.Cells["A2"].PutValue(100);
worksheet.Cells["A3"].PutValue(150);
worksheet.Cells["A4"].PutValue(200);
worksheet.Cells["B1"].PutValue(60);
worksheet.Cells["B2"].PutValue(32);
worksheet.Cells["B3"].PutValue(50);
worksheet.Cells["B4"].PutValue(40);
// Create chart
int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Line, 5, 0, 15, 5);
Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
chart.NSeries.Add("A1:B4", true);
// Add trendline and get it by index
int trendlineIndex = chart.NSeries[0].TrendLines.Add(Aspose.Cells.Charts.TrendlineType.Linear);
Aspose.Cells.Charts.Trendline trendline = chart.NSeries[0].TrendLines[trendlineIndex];
trendline.Name = "Linear Trend";
trendline.DisplayEquation = true;
// Set backward property to extend trendline backward by 0.5 units
trendline.Backward = 0.5;
workbook.Save("TrendlineBackwardDemo.xlsx");
}
}
}
```
### See Also
* class [Trendline](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
