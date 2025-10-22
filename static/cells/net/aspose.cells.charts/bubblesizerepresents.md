##Enum BubbleSizeRepresents
Aspose.Cells.Charts.BubbleSizeRepresents enum. Represents what the bubble size represents on a bubble chart
## BubbleSizeRepresents enumeration
Represents what the bubble size represents on a bubble chart.
```csharp
public enum BubbleSizeRepresents
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| SizeIsArea | `0` | Represents the value of [`BubbleSizes`](../series/bubblesizes/) is area of the bubble. |
| SizeIsWidth | `1` | Represents the value of [`BubbleSizes`](../series/bubblesizes/) is width of the bubble. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using System;
public class BubbleSizeRepresentsDemo
{
public static void BubbleSizeRepresentsExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add a new worksheet to the workbook
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for the bubble chart
worksheet.Cells["A1"].PutValue(1);
worksheet.Cells["A2"].PutValue(2);
worksheet.Cells["A3"].PutValue(3);
worksheet.Cells["B1"].PutValue(2);
worksheet.Cells["B2"].PutValue(3);
worksheet.Cells["B3"].PutValue(4);
worksheet.Cells["C1"].PutValue(5);
worksheet.Cells["C2"].PutValue(10);
worksheet.Cells["C3"].PutValue(15);
// Add a bubble chart to the worksheet
int chartIndex = worksheet.Charts.Add(ChartType.Bubble, 5, 0, 15, 5);
Chart chart = worksheet.Charts[chartIndex];
// Add series to the bubble chart
int seriesIndex = chart.NSeries.Add("A1:C3", true);
Series series = chart.NSeries[seriesIndex];
// Set the X values, Y values, and bubble sizes
series.XValues = "A1:A3";
series.Values = "B1:B3";
series.BubbleSizes = "C1:C3";
// Set the bubble size representation
series.SizeRepresents = BubbleSizeRepresents.SizeIsArea;
// Save the workbook
workbook.Save("BubbleSizeRepresentsExample.xlsx");
workbook.Save("BubbleSizeRepresentsExample.pdf");
// Set the bubble size representation
series.SizeRepresents = BubbleSizeRepresents.SizeIsWidth;
// Save the workbook
workbook.Save("BubbleSizeRepresentsExample2.xlsx");
workbook.Save("BubbleSizeRepresentsExample2.pdf");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)
