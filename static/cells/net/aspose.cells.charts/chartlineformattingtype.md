##Enum ChartLineFormattingType
Aspose.Cells.Charts.ChartLineFormattingType enum. Represents line format type of chart line
## ChartLineFormattingType enumeration
Represents line format type of chart line.
```csharp
public enum ChartLineFormattingType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Automatic | `0` | Represents automatic formatting type. |
| Solid | `1` | Represents solid formatting type. |
| None | `2` | Represents none formatting type. |
| Gradient | `3` | Gradient |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using System;
using System.Drawing;
public class ChartLineFormattingTypeDemo
{
public static void ChartLineFormattingTypeExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add a new worksheet to the workbook
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to cells
worksheet.Cells["A1"].PutValue(50);
worksheet.Cells["A2"].PutValue(100);
worksheet.Cells["A3"].PutValue(150);
worksheet.Cells["B1"].PutValue(60);
worksheet.Cells["B2"].PutValue(32);
worksheet.Cells["B3"].PutValue(50);
// Add a chart to the worksheet
int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 15, 5);
Chart chart = worksheet.Charts[chartIndex];
// Add series to the chart
chart.NSeries.Add("A1:B3", true);
// Set the category data
chart.NSeries.CategoryData = "A1:A3";
// Set different line formatting types for the series
chart.NSeries[0].SeriesLines.FormattingType = ChartLineFormattingType.Solid;
chart.NSeries[0].SeriesLines.Color = Color.Red;
// Add another series with different formatting
chart.NSeries.Add("B1:B3", true);
chart.NSeries[1].SeriesLines.FormattingType = ChartLineFormattingType.Gradient;
chart.NSeries[1].SeriesLines.Color = Color.Blue;
// Save the workbook
workbook.Save("ChartLineFormattingTypeExample.xlsx");
workbook.Save("ChartLineFormattingTypeExample.pdf");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)
