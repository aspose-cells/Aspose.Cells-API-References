##Series.HasDropLines
Series property. True if the chart has drop lines. Applies only to line chart or area charts
## Series.HasDropLines property
True if the chart has drop lines. Applies only to line chart or area charts.
```csharp
public bool HasDropLines { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class SeriesPropertyHasDropLinesDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["A2"].PutValue("A");
worksheet.Cells["A3"].PutValue("B");
worksheet.Cells["A4"].PutValue("C");
worksheet.Cells["B1"].PutValue("Value");
worksheet.Cells["B2"].PutValue(10);
worksheet.Cells["B3"].PutValue(20);
worksheet.Cells["B4"].PutValue(30);
// Add a line chart
int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 20, 10);
Chart chart = worksheet.Charts[chartIndex];
// Add series data
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
// Get the first series
Series series = chart.NSeries[0];
// Demonstrate HasDropLines property
series.HasDropLines = true; // Enable drop lines
series.Type = ChartType.Line; // Ensure it's a line chart for drop lines to be visible
// Save the workbook
workbook.Save("SeriesHasDropLinesDemo.xlsx");
}
}
}
```
### See Also
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
