##Series.DropLines
Series property. Returns a Line object that represents the drop lines for a series on the line chart or area chart. Applies only to line chart or area charts
## Series.DropLines property
Returns a [`Line`](../../../aspose.cells.drawing/line/) object that represents the drop lines for a series on the line chart or area chart. Applies only to line chart or area charts.
```csharp
public Line DropLines { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System;
public class SeriesPropertyDropLinesDemo
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
worksheet.Cells["B1"].PutValue("Series 1");
worksheet.Cells["B2"].PutValue(120);
worksheet.Cells["B3"].PutValue(150);
worksheet.Cells["B4"].PutValue(180);
worksheet.Cells["B5"].PutValue(210);
worksheet.Cells["C1"].PutValue("Series 2");
worksheet.Cells["C2"].PutValue(90);
worksheet.Cells["C3"].PutValue(130);
worksheet.Cells["C4"].PutValue(160);
worksheet.Cells["C5"].PutValue(190);
// Add a line chart
int chartIndex = worksheet.Charts.Add(ChartType.Line, 6, 0, 20, 10);
Chart chart = worksheet.Charts[chartIndex];
// Set chart data range
chart.NSeries.Add("B2:B5", true);
chart.NSeries.Add("C2:C5", true);
chart.NSeries.CategoryData = "A2:A5";
// Enable drop lines for the chart
chart.NSeries[0].HasDropLines = true;
chart.NSeries[1].HasDropLines = true;
// Access the drop lines for the first series
Line dropLines = chart.NSeries[0].DropLines;
// Display current drop line properties
Console.WriteLine("Drop line color: " + dropLines.Color);
Console.WriteLine("Drop line style: " + dropLines.Style);
Console.WriteLine("Drop line weight: " + dropLines.Weight);
// Modify drop line properties
dropLines.Color = System.Drawing.Color.Red;
dropLines.Style = LineType.Solid;
dropLines.Weight = WeightType.MediumLine;
dropLines.DashType = MsoLineDashStyle.Solid;
dropLines.IsVisible = true;
// Save the workbook
workbook.Save("SeriesPropertyDropLinesDemo.xlsx");
}
}
}
```
### See Also
* class [Line](../../../aspose.cells.drawing/line/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
