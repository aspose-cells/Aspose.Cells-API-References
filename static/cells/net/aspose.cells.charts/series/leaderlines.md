##Series.LeaderLines
Series property. Represents leader lines on a chart. Leader lines connect data labels to data points. This object isnt a collection theres no object that represents a single leader line
## Series.LeaderLines property
Represents leader lines on a chart. Leader lines connect data labels to data points. This object isn’t a collection; there’s no object that represents a single leader line.
```csharp
public Line LeaderLines { get; }
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
public class SeriesPropertyLeaderLinesDemo
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
worksheet.Cells["B1"].PutValue("Value");
worksheet.Cells["B2"].PutValue(10);
worksheet.Cells["B3"].PutValue(20);
worksheet.Cells["B4"].PutValue(30);
// Add a pie chart
int chartIndex = worksheet.Charts.Add(ChartType.Pie, 5, 0, 20, 8);
Chart chart = worksheet.Charts[chartIndex];
// Set chart data range
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
// Configure data labels
Series series = chart.NSeries[0];
series.DataLabels.ShowValue = true;
series.DataLabels.ShowPercentage = true;
series.DataLabels.Position = LabelPositionType.OutsideEnd;
// Configure leader lines
series.HasLeaderLines = true;
series.LeaderLines.IsAuto = false;
series.LeaderLines.Style = LineType.Dot;
series.LeaderLines.WeightPt = 1.5;
series.LeaderLines.Color = Color.Blue;
// Save the workbook
workbook.Save("SeriesPropertyLeaderLinesDemo_out.xlsx");
}
}
}
```
### See Also
* class [Line](../../../aspose.cells.drawing/line/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
