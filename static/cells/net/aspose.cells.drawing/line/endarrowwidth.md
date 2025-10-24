##Line.EndArrowWidth
Line property. Specifies the width of the arrowhead for the end of a line
## Line.EndArrowWidth property
Specifies the width of the arrowhead for the end of a line.
```csharp
public MsoArrowheadWidth EndArrowWidth { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class LinePropertyEndArrowWidthDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for line chart
worksheet.Cells["A1"].PutValue(1);
worksheet.Cells["A2"].PutValue(2);
worksheet.Cells["A3"].PutValue(3);
worksheet.Cells["B1"].PutValue(4);
worksheet.Cells["B2"].PutValue(5);
worksheet.Cells["B3"].PutValue(6);
// Add a line chart
int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 15, 5);
Chart chart = worksheet.Charts[chartIndex];
// Set chart data source
chart.NSeries.Add("A1:B3", true);
// Configure line properties for the first series
Series series = chart.NSeries[0];
series.Border.EndArrowWidth = MsoArrowheadWidth.Wide;
series.Border.EndType = MsoArrowheadStyle.Arrow;
// Save the workbook
workbook.Save("LinePropertyEndArrowWidthDemo.xlsx");
}
}
}
```
### See Also
* enum [MsoArrowheadWidth](../../msoarrowheadwidth/)
* class [Line](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
