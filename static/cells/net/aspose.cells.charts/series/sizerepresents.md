##Series.SizeRepresents
Series property. Gets or sets what the bubble size represents on a bubble chart
## Series.SizeRepresents property
Gets or sets what the bubble size represents on a bubble chart.
```csharp
public BubbleSizeRepresents SizeRepresents { get; set; }
```
### Remarks
BubbleSizeRepresents.SizeIsArea means the value [`BubbleSizes`](../bubblesizes/) is the area of the bubble. BubbleSizeRepresents.SizeIsWidth means the value [`BubbleSizes`](../bubblesizes/) is the width of the bubble.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class SeriesPropertySizeRepresentsDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add sample data for bubble chart
sheet.Cells["A1"].PutValue("X");
sheet.Cells["B1"].PutValue("Y");
sheet.Cells["C1"].PutValue("Size");
for (int i = 2; i <= 5; i++)
{
sheet.Cells["A" + i].PutValue(i);
sheet.Cells["B" + i].PutValue(i * 2);
sheet.Cells["C" + i].PutValue(i * 0.5);
}
// Add a bubble chart
int chartIndex = sheet.Charts.Add(ChartType.Bubble, 5, 0, 20, 8);
Chart chart = sheet.Charts[chartIndex];
// Set series data
SeriesCollection series = chart.NSeries;
series.Add("B2:B5", true);
series.CategoryData = "A2:A5";
series[0].BubbleSizes = "C2:C5";
// Set SizeRepresents property
series[0].SizeRepresents = BubbleSizeRepresents.SizeIsArea;
// Save the workbook
workbook.Save("SeriesPropertySizeRepresentsDemo.xlsx");
}
}
}
```
### See Also
* enum [BubbleSizeRepresents](../../bubblesizerepresents/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
