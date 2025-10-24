##Enum LineJoinType
Aspose.Cells.Drawing.LineJoinType enum. Represents the join styles of a line
## LineJoinType enumeration
Represents the join styles of a line.
```csharp
public enum LineJoinType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Round | `0` | Round joint |
| Bevel | `1` | Bevel joint |
| Miter | `2` | Miter joint |
| None | `3` | None joint |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System;
public class LineJoinTypeDemo
{
public static void LineJoinTypeExample()
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
// Access the primary value axis
Axis valueAxis = chart.ValueAxis;
// Access the line format of the major gridlines
Line majorGridLines = valueAxis.MajorGridLines;
// Set the join type of the line
majorGridLines.JoinType = LineJoinType.Round;
// Output the join type
Console.WriteLine("Line Join Type: " + majorGridLines.JoinType);
// Save the workbook
workbook.Save("LineJoinTypeExample.xlsx");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)
