##Enum LineType
Aspose.Cells.Drawing.LineType enum. Enumerates the type of Picture border or Chart line
## LineType enumeration
Enumerates the type of [`Picture`](../picture/) border or [`Chart`](../../aspose.cells.charts/chart/) line.
```csharp
public enum LineType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| DarkGray | `6` | Represents a dark gray line. |
| Dash | `1` | Represent a dash line. |
| DashDot | `3` | Represents a dash-dot line |
| DashDotDot | `4` | Represents a dash-dot-dot line. |
| Dot | `2` | Represents a dotted line. |
| LightGray | `8` | Represents a light gray line. |
| MediumGray | `7` | Represents a medium gray line. |
| Solid | `0` | Represent a solid line. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System;
using System.Drawing;
public class LineTypeDemo
{
public static void LineTypeExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add a new worksheet to the workbook
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to the worksheet
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["A2"].PutValue("A");
worksheet.Cells["A3"].PutValue("B");
worksheet.Cells["A4"].PutValue("C");
worksheet.Cells["B1"].PutValue("Value");
worksheet.Cells["B2"].PutValue(10);
worksheet.Cells["B3"].PutValue(20);
worksheet.Cells["B4"].PutValue(30);
// Add a chart to the worksheet
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
Chart chart = worksheet.Charts[chartIndex];
// Set the chart data range
chart.SetChartDataRange("A1:B4", true);
// Access the primary category axis
Axis categoryAxis = chart.CategoryAxis;
// Set the line type for the axis line
categoryAxis.AxisLine.Style = LineType.DashDot;
// Set the color of the axis line
categoryAxis.AxisLine.Color = Color.Blue;
// Access the primary value axis
Axis valueAxis = chart.ValueAxis;
// Set the line type for the major gridlines
valueAxis.MajorGridLines.Style = LineType.Dot;
// Set the color of the major gridlines
valueAxis.MajorGridLines.Color = Color.Red;
// Save the workbook
workbook.Save("LineTypeExample.xlsx");
// Output the results
Console.WriteLine("Chart created with custom line types for axis and gridlines.");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)
