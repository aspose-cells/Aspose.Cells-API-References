##Series.HasSeriesLines
Series property. True if a stacked column chart or bar chart has series lines or if a Pie of Pie chart or Bar of Pie chart has connector lines between the two sections. Applies only to stacked column charts bar charts Pie of Pie charts or Bar of Pie charts
## Series.HasSeriesLines property
True if a stacked column chart or bar chart has series lines or if a Pie of Pie chart or Bar of Pie chart has connector lines between the two sections. Applies only to stacked column charts, bar charts, Pie of Pie charts, or Bar of Pie charts.
```csharp
public bool HasSeriesLines { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class SeriesPropertyHasSeriesLinesDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue(50);
worksheet.Cells["A2"].PutValue(100);
worksheet.Cells["A3"].PutValue(150);
worksheet.Cells["B1"].PutValue(60);
worksheet.Cells["B2"].PutValue(32);
worksheet.Cells["B3"].PutValue(50);
worksheet.Cells["C1"].PutValue("Q1");
worksheet.Cells["C2"].PutValue("Q2");
worksheet.Cells["C3"].PutValue("Q3");
// Add a stacked column chart
int chartIndex = worksheet.Charts.Add(ChartType.ColumnStacked, 5, 0, 15, 5);
Chart chart = worksheet.Charts[chartIndex];
// Add series data
chart.NSeries.Add("A1:B3", true);
chart.NSeries.CategoryData = "C1:C3";
// Access the first series
Series series = chart.NSeries[0];
// Demonstrate HasSeriesLines property
series.HasSeriesLines = true; // Enable series lines
// Save the workbook
workbook.Save("SeriesHasSeriesLinesDemo.xlsx");
}
}
}
```
### See Also
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
