##Enum MsoLineStyle
Aspose.Cells.Drawing.MsoLineStyle enum. Represents style of drawing lines
## MsoLineStyle enumeration
Represents style of drawing lines.
```csharp
public enum MsoLineStyle
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Single | `0` | Single line (of width lineWidth) |
| ThickBetweenThin | `1` | Three lines, thin, thick, thin |
| ThinThick | `2` | Double lines, one thin, one thick |
| ThickThin | `3` | Double lines, one thick, one thin |
| ThinThin | `4` | Double lines of equal width |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System;
using System.Drawing;
public class MsoLineStyleDemo
{
public static void MsoLineStyleExample()
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
// Set the line style for the primary category axis
Line axisLine = categoryAxis.AxisLine;
axisLine.CompoundType = MsoLineStyle.ThickBetweenThin;
axisLine.Color = Color.Blue;
axisLine.WeightPt = 2.0;
// Output the line style
Console.WriteLine("Axis Line Style: " + axisLine.CompoundType);
Console.WriteLine("Axis Line Color: " + axisLine.Color);
Console.WriteLine("Axis Line Weight: " + axisLine.WeightPt);
// Save the workbook
workbook.Save("MsoLineStyleExample.xlsx");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)
