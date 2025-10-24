##Series.ShowNegativeBubbles
Series property. True if negative bubbles are shown for the chart group. Valid only for bubble charts
## Series.ShowNegativeBubbles property
True if negative bubbles are shown for the chart group. Valid only for bubble charts.
```csharp
public bool ShowNegativeBubbles { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class SeriesPropertyShowNegativeBubblesDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for bubble chart
worksheet.Cells["A1"].PutValue("X");
worksheet.Cells["A2"].PutValue(1);
worksheet.Cells["A3"].PutValue(2);
worksheet.Cells["A4"].PutValue(3);
worksheet.Cells["B1"].PutValue("Y");
worksheet.Cells["B2"].PutValue(2);
worksheet.Cells["B3"].PutValue(-3);
worksheet.Cells["B4"].PutValue(4);
worksheet.Cells["C1"].PutValue("Size");
worksheet.Cells["C2"].PutValue(5);
worksheet.Cells["C3"].PutValue(6);
worksheet.Cells["C4"].PutValue(7);
// Add a bubble chart
int chartIndex = worksheet.Charts.Add(ChartType.Bubble, 5, 0, 20, 8);
Chart chart = worksheet.Charts[chartIndex];
// Set chart data range
SeriesCollection seriesCollection = chart.NSeries;
seriesCollection.Add("B2:B4", true);
seriesCollection.CategoryData = "A2:A4";
seriesCollection[0].BubbleSizes = "C2:C4";
// Access the first series and set ShowNegativeBubbles property
Series series = chart.NSeries[0];
series.ShowNegativeBubbles = true;
// Save the workbook
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
