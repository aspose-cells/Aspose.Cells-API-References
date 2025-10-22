##Series.SplitType
Series property. Returns or sets a value that how to determine which data points are in the second pie or bar on a pie of pie or bar of pie chart
## Series.SplitType property
Returns or sets a value that how to determine which data points are in the second pie or bar on a pie of pie or bar of pie chart.
```csharp
public ChartSplitType SplitType { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class SeriesPropertySplitTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add sample data for chart
sheet.Cells["A1"].PutValue("Category");
sheet.Cells["A2"].PutValue("A");
sheet.Cells["A3"].PutValue("B");
sheet.Cells["A4"].PutValue("C");
sheet.Cells["B1"].PutValue("Value");
sheet.Cells["B2"].PutValue(10);
sheet.Cells["B3"].PutValue(20);
sheet.Cells["B4"].PutValue(30);
// Add a pie chart
int chartIndex = sheet.Charts.Add(ChartType.Pie, 5, 0, 20, 8);
Chart chart = sheet.Charts[chartIndex];
// Set chart data range
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
// Set split type for the first series
chart.NSeries[0].SplitType = ChartSplitType.Position;
// Save the workbook
workbook.Save("SeriesPropertySplitTypeDemo_out.xlsx");
}
}
}
```
### See Also
* enum [ChartSplitType](../../chartsplittype/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
