##Series.HiLoLines
Series property. Returns a HiLoLines object that represents the highlow lines for a series on a line chart. Applies only to line charts
## Series.HiLoLines property
Returns a HiLoLines object that represents the high-low lines for a series on a line chart. Applies only to line charts.
```csharp
public Line HiLoLines { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System;
public class SeriesPropertyHiLoLinesDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for the chart
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["A2"].PutValue("Q1");
worksheet.Cells["A3"].PutValue("Q2");
worksheet.Cells["A4"].PutValue("Q3");
worksheet.Cells["A5"].PutValue("Q4");
worksheet.Cells["B1"].PutValue("High");
worksheet.Cells["B2"].PutValue(120);
worksheet.Cells["B3"].PutValue(90);
worksheet.Cells["B4"].PutValue(150);
worksheet.Cells["B5"].PutValue(110);
worksheet.Cells["C1"].PutValue("Low");
worksheet.Cells["C2"].PutValue(80);
worksheet.Cells["C3"].PutValue(60);
worksheet.Cells["C4"].PutValue(100);
worksheet.Cells["C5"].PutValue(70);
// Add a line chart
int chartIndex = worksheet.Charts.Add(ChartType.Line, 6, 0, 20, 10);
Chart chart = worksheet.Charts[chartIndex];
// Set chart data range
chart.NSeries.Add("B1:B5", true);
chart.NSeries.Add("C1:C5", true);
chart.NSeries.CategoryData = "A2:A5";
// Enable HiLoLines for the first series
Series series = chart.NSeries[0];
series.HasHiLoLines = true;
// Access and modify HiLoLines properties
Line hiLoLines = series.HiLoLines;
Console.WriteLine("HiLoLines visibility: " + hiLoLines.IsVisible);
// Customize HiLoLines appearance
hiLoLines.Color = System.Drawing.Color.Red;
hiLoLines.Weight = WeightType.MediumLine;
hiLoLines.DashType = MsoLineDashStyle.DashDot;
hiLoLines.IsVisible = true;
// Save the result
workbook.Save("SeriesPropertyHiLoLinesDemo.xlsx");
}
}
}
```
### See Also
* class [Line](../../../aspose.cells.drawing/line/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
