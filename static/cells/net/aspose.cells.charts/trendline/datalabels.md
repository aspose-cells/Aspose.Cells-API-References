##Trendline.DataLabels
Trendline property. Represents the DataLabels object for the specified series
## Trendline.DataLabels property
Represents the DataLabels object for the specified series.
```csharp
public DataLabels DataLabels { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System.Drawing;
namespace AsposeCellsExamples
{
public class TrendlinePropertyDataLabelsDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add sample data
sheet.Cells["A1"].PutValue("X Values");
sheet.Cells["B1"].PutValue("Y Values");
for (int i = 2; i <= 10; i++)
{
sheet.Cells["A" + i].PutValue(i);
sheet.Cells["B" + i].PutValue(i * 2);
}
// Create chart
int chartIndex = sheet.Charts.Add(ChartType.Scatter, 5, 0, 20, 10);
Chart chart = sheet.Charts[chartIndex];
// Add series and set trendline
chart.NSeries.Add("B2:B10", true);
chart.NSeries[0].XValues = "A2:A10";
chart.NSeries[0].TrendLines.Add(TrendlineType.Linear, "Linear Trend");
// Configure DataLabels for trendline
Trendline trendline = chart.NSeries[0].TrendLines[0];
trendline.DataLabels.ShowValue = true;
trendline.DataLabels.Font.Color = Color.Red;
trendline.DataLabels.Font.IsBold = true;
trendline.DataLabels.Position = LabelPositionType.Above;
trendline.DataLabels.Border.IsVisible = true;
trendline.DataLabels.Border.Color = Color.Black;
// Save the workbook
workbook.Save("TrendlineDataLabelsDemo.xlsx");
}
}
}
```
### See Also
* class [DataLabels](../../datalabels/)
* class [Trendline](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
