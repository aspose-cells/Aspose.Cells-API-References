##Line.BeginArrowWidth
Line property. Specifies the width of the arrowhead for the begin of a line
## Line.BeginArrowWidth property
Specifies the width of the arrowhead for the begin of a line.
```csharp
public MsoArrowheadWidth BeginArrowWidth { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class LinePropertyBeginArrowWidthDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue(50);
worksheet.Cells["A2"].PutValue(100);
worksheet.Cells["A3"].PutValue(150);
worksheet.Cells["B1"].PutValue(60);
worksheet.Cells["B2"].PutValue(32);
worksheet.Cells["B3"].PutValue(50);
// Add chart
int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 15, 5);
Chart chart = worksheet.Charts[chartIndex];
chart.NSeries.Add("A1:B3", true);
// Add trendline and set arrow properties
int trendlineIndex = chart.NSeries[0].TrendLines.Add(TrendlineType.Linear);
Trendline trendline = chart.NSeries[0].TrendLines[trendlineIndex];
trendline.BeginType = MsoArrowheadStyle.Arrow;
trendline.BeginArrowWidth = MsoArrowheadWidth.Wide;
trendline.EndType = MsoArrowheadStyle.Arrow;
trendline.EndArrowWidth = MsoArrowheadWidth.Narrow;
workbook.Save("LinePropertyBeginArrowWidthDemo.xlsx");
}
}
}
```
### See Also
* enum [MsoArrowheadWidth](../../msoarrowheadwidth/)
* class [Line](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
