##Line.FormattingType
Line property. Gets or sets format type
## Line.FormattingType property
Gets or sets format type.
```csharp
public ChartLineFormattingType FormattingType { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using System.Drawing;
namespace AsposeCellsExamples
{
public class LinePropertyFormattingTypeDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue(50);
worksheet.Cells["A2"].PutValue(100);
worksheet.Cells["A3"].PutValue(150);
worksheet.Cells["B1"].PutValue(60);
worksheet.Cells["B2"].PutValue(32);
worksheet.Cells["B3"].PutValue(50);
int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 15, 5);
Chart chart = worksheet.Charts[chartIndex];
chart.NSeries.Add("A1:B3", true);
chart.NSeries.CategoryData = "A1:A3";
chart.NSeries[0].SeriesLines.FormattingType = ChartLineFormattingType.Solid;
chart.NSeries[0].SeriesLines.Color = Color.Red;
chart.NSeries[1].SeriesLines.FormattingType = ChartLineFormattingType.Gradient;
chart.NSeries[1].SeriesLines.Color = Color.Blue;
workbook.Save("LinePropertyFormattingTypeDemo.xlsx");
}
}
}
```
### See Also
* enum [ChartLineFormattingType](../../../aspose.cells.charts/chartlineformattingtype/)
* class [Line](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
