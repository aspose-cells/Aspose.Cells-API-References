##Enum MsoLineDashStyle
Aspose.Cells.Drawing.MsoLineDashStyle enum. Represents style of dash drawing lines
## MsoLineDashStyle enumeration
Represents style of dash drawing lines.
```csharp
public enum MsoLineDashStyle
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Dash | `0` | Represent a dash line. |
| DashDot | `1` | Represents a dash-dot line. |
| DashDotDot | `2` | Represents a dash-dot-dot line. |
| DashLongDash | `3` | Represents a long dash-short dash line. |
| DashLongDashDot | `4` | Represents a long dash-short dash-dot line. |
| RoundDot | `5` | Represents a round-dot line. |
| Solid | `6` | Represent a solid line. |
| SquareDot | `7` | Represents a square-dot line. |
| Custom | `8` | Custom dash style. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System;
public class MsoLineDashStyleDemo
{
public static void MsoLineDashStyleExample()
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
// Set the dash style of the major gridlines
categoryAxis.MajorGridLines.DashType = MsoLineDashStyle.DashDot;
// Set the dash style of the minor gridlines
categoryAxis.MinorGridLines.DashType = MsoLineDashStyle.DashLongDashDot;
// Save the workbook
workbook.Save("MsoLineDashStyleExample.xlsx");
// Output the results
Console.WriteLine("Chart with custom dash styles for gridlines created successfully.");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)
