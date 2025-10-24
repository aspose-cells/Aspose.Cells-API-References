##Series.SecondPlotSize
Series property. Returns or sets the size of the secondary section of either a pie of pie chart or a bar of pie chart as a percentage of the size of the primary pie. Can be a value from 5 to 200
## Series.SecondPlotSize property
Returns or sets the size of the secondary section of either a pie of pie chart or a bar of pie chart, as a percentage of the size of the primary pie. Can be a value from 5 to 200.
```csharp
public short SecondPlotSize { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class SeriesPropertySecondPlotSizeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for pie chart
worksheet.Cells["A1"].PutValue("Fruit");
worksheet.Cells["A2"].PutValue("Apple");
worksheet.Cells["A3"].PutValue("Orange");
worksheet.Cells["A4"].PutValue("Banana");
worksheet.Cells["B1"].PutValue("Quantity");
worksheet.Cells["B2"].PutValue(50);
worksheet.Cells["B3"].PutValue(30);
worksheet.Cells["B4"].PutValue(20);
// Add a pie chart
int chartIndex = worksheet.Charts.Add(ChartType.Pie, 5, 0, 20, 8);
Chart chart = worksheet.Charts[chartIndex];
// Set chart data range
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
// Get the first series
Series series = chart.NSeries[0];
// Set SecondPlotSize property (percentage of pie to show in second plot)
series.SecondPlotSize = 30; // 30% of the pie will be shown in second plot
// Save the workbook
workbook.Save("SeriesPropertySecondPlotSizeDemo_out.xlsx");
}
}
}
```
### See Also
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
