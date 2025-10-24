##Enum ChartMarkerType
Aspose.Cells.Charts.ChartMarkerType enum. Represents the marker style in a line chart scatter chart or radar chart
## ChartMarkerType enumeration
Represents the marker style in a line chart, scatter chart, or radar chart.
```csharp
public enum ChartMarkerType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Automatic | `0` | Automatic markers. |
| Circle | `1` | Circular markers. |
| Dash | `2` | Long bar markers |
| Diamond | `3` | Diamond-shaped markers. |
| Dot | `4` | Short bar markers. |
| None | `5` | No markers. |
| SquarePlus | `6` | Square markers with a plus sign. |
| Square | `7` | Square markers. |
| SquareStar | `8` | Square markers with an asterisk. |
| Triangle | `9` | Triangular markers. |
| SquareX | `10` | Square markers with an X. |
| Picture | `11` | Picture |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using System;
using System.Drawing;
public class ChartMarkerTypeDemo
{
public static void ChartMarkerTypeExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for the chart
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["A2"].PutValue("A");
worksheet.Cells["A3"].PutValue("B");
worksheet.Cells["A4"].PutValue("C");
worksheet.Cells["B1"].PutValue("Value");
worksheet.Cells["B2"].PutValue(10);
worksheet.Cells["B3"].PutValue(20);
worksheet.Cells["B4"].PutValue(30);
// Add a chart to the worksheet
int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 20, 10);
Chart chart = worksheet.Charts[chartIndex];
// Add the data series to the chart
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
// Access the marker of the first series
Marker marker = chart.NSeries[0].Marker;
// Set the marker style
marker.MarkerStyle = ChartMarkerType.Circle;
// Set the marker size
marker.MarkerSize = 10;
// Set the marker foreground and background colors
marker.ForegroundColor = Color.Red;
marker.BackgroundColor = Color.Yellow;
// Save the workbook
workbook.Save("ChartMarkerTypeExample.xlsx");
workbook.Save("ChartMarkerTypeExample.pdf");
return;
}
}
}
```
### See Also
* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)
