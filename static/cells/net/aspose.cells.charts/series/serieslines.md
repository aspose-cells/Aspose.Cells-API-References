##Series.SeriesLines
Series property. Returns a SeriesLines object that represents the series lines for a stacked bar chart or a stacked column chart. Applies only to stacked bar and stacked column charts
## Series.SeriesLines property
Returns a SeriesLines object that represents the series lines for a stacked bar chart or a stacked column chart. Applies only to stacked bar and stacked column charts.
```csharp
public Line SeriesLines { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;
namespace AsposeCellsExamples
{
public class SeriesPropertySeriesLinesDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("X");
worksheet.Cells["A2"].PutValue(1);
worksheet.Cells["A3"].PutValue(2);
worksheet.Cells["A4"].PutValue(3);
worksheet.Cells["A5"].PutValue(4);
worksheet.Cells["B1"].PutValue("Y");
worksheet.Cells["B2"].PutValue(10);
worksheet.Cells["B3"].PutValue(20);
worksheet.Cells["B4"].PutValue(30);
worksheet.Cells["B5"].PutValue(40);
// Create chart
int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Line, 5, 0, 20, 10);
Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
// Add series
chart.NSeries.Add("B2:B5", true);
chart.NSeries.CategoryData = "A2:A5";
// Customize series lines
Aspose.Cells.Charts.Series series = chart.NSeries[0];
series.SeriesLines.Color = Color.Red;
series.SeriesLines.Weight = Aspose.Cells.Drawing.WeightType.SingleLine;
// Save the workbook
workbook.Save("SeriesLinesDemo.xlsx");
}
}
}
```
### See Also
* class [Line](../../../aspose.cells.drawing/line/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
