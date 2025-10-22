##DataLabels.ShowBubbleSize
DataLabels property. Represents a specified charts data label percentage value display behavior. True displays the percentage value. False to hide
## DataLabels.ShowBubbleSize property
Represents a specified chart's data label percentage value display behavior. True displays the percentage value. False to hide.
```csharp
public bool ShowBubbleSize { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class DataLabelsPropertyShowBubbleSizeDemo
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
worksheet.Cells["B2"].PutValue(10);
worksheet.Cells["B3"].PutValue(20);
worksheet.Cells["B4"].PutValue(30);
worksheet.Cells["C1"].PutValue("Size");
worksheet.Cells["C2"].PutValue(5);
worksheet.Cells["C3"].PutValue(10);
worksheet.Cells["C4"].PutValue(15);
// Add a bubble chart
int chartIndex = worksheet.Charts.Add(ChartType.Bubble, 5, 0, 20, 8);
Chart chart = worksheet.Charts[chartIndex];
// Add series to the chart
int seriesIndex = chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
// Set bubble sizes for the series
Series series = chart.NSeries[seriesIndex];
series.BubbleSizes = "C2:C4";
// Access the DataLabels of the series
DataLabels dataLabels = series.DataLabels;
// Demonstrate ShowBubbleSize property
dataLabels.ShowBubbleSize = true; // Show bubble size in data labels
dataLabels.ShowValue = true;      // Also show values for clarity
// Save the workbook
workbook.Save("DataLabelsShowBubbleSizeDemo.xlsx");
}
}
}
```
### See Also
* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
