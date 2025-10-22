##Series.Points
Series property. Gets the collection of points in a series in a chart
## Series.Points property
Gets the collection of points in a series in a chart.
```csharp
public ChartPointCollection Points { get; }
```
### Remarks
When the chart is Pie of Pie or Bar of Pie, the last point is other point in first pie plot.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class SeriesPropertyPointsDemo
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
// Add a chart
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
Chart chart = worksheet.Charts[chartIndex];
// Set chart data range
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
// Access the first series and its points
Series series = chart.NSeries[0];
foreach (ChartPoint point in series.Points)
{
// Add data labels to each point
point.DataLabels.ShowValue = true;
point.DataLabels.ShowCellRange = true;
}
// Save the workbook
workbook.Save("SeriesPropertyPointsDemo_Output.xlsx");
}
}
}
```
### See Also
* class [ChartPointCollection](../../chartpointcollection/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
