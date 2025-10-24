##Series.BubbleSizes
Series property. Gets or sets the bubble sizes values of the chart series
## Series.BubbleSizes property
Gets or sets the bubble sizes values of the chart series.
```csharp
public string BubbleSizes { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class SeriesPropertyBubbleSizesDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for bubble chart
worksheet.Cells["A1"].PutValue("X Values");
worksheet.Cells["B1"].PutValue("Y Values");
worksheet.Cells["C1"].PutValue("Bubble Sizes");
for (int i = 2; i <= 5; i++)
{
worksheet.Cells["A" + i].PutValue(i);
worksheet.Cells["B" + i].PutValue(i * 2);
worksheet.Cells["C" + i].PutValue(i * 0.5);
}
// Add a bubble chart
int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Bubble, 5, 0, 20, 8);
Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
// Set series data using BubbleSizes property
chart.NSeries.Add("A2:A5", true);
chart.NSeries[0].XValues = "B2:B5";
chart.NSeries[0].BubbleSizes = "C2:C5";
// Save the workbook
workbook.Save("BubbleChartDemo.xlsx");
}
}
}
```
### See Also
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
