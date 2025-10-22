##Line.EndType
Line property. Specifies an arrowhead for the end of a line
## Line.EndType property
Specifies an arrowhead for the end of a line.
```csharp
public MsoArrowheadStyle EndType { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class LinePropertyEndTypeDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue(50);
worksheet.Cells["A2"].PutValue(100);
worksheet.Cells["A3"].PutValue(150);
worksheet.Cells["A4"].PutValue(200);
worksheet.Cells["B1"].PutValue(60);
worksheet.Cells["B2"].PutValue(32);
worksheet.Cells["B3"].PutValue(50);
worksheet.Cells["B4"].PutValue(40);
// Add chart
int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 15, 5);
Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
chart.NSeries.Add("A1:B4", true);
// Add trendline and set EndType
int trendlineIndex = chart.NSeries[0].TrendLines.Add(TrendlineType.Linear);
Aspose.Cells.Charts.Trendline trendline = chart.NSeries[0].TrendLines[trendlineIndex];
trendline.EndType = MsoArrowheadStyle.Arrow;
trendline.EndArrowLength = MsoArrowheadLength.Medium;
trendline.EndArrowWidth = MsoArrowheadWidth.Medium;
workbook.Save("LineEndTypeDemo.xlsx");
}
}
}
```
### See Also
* enum [MsoArrowheadStyle](../../msoarrowheadstyle/)
* class [Line](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
