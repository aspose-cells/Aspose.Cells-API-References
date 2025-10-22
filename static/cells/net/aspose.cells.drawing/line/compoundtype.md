##Line.CompoundType
Line property. Specifies the compound line type
## Line.CompoundType property
Specifies the compound line type
```csharp
public MsoLineStyle CompoundType { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class LinePropertyCompoundTypeDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue(1);
worksheet.Cells["A2"].PutValue(2);
worksheet.Cells["A3"].PutValue(3);
int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 15, 5);
Chart chart = worksheet.Charts[chartIndex];
chart.NSeries.Add("A1:A3", true);
Series series = chart.NSeries[0];
int trendlineIndex = series.TrendLines.Add(TrendlineType.Linear);
Trendline trendline = series.TrendLines[trendlineIndex];
trendline.CapType = LineCapType.Round;
trendline.CompoundType = MsoLineStyle.ThickThin;
trendline.IsVisible = true;
trendline.DisplayEquation = true;
Console.WriteLine("CompoundType: " + trendline.CompoundType);
workbook.Save("LinePropertyCompoundTypeDemo_out.xlsx");
}
}
}
```
### See Also
* enum [MsoLineStyle](../../msolinestyle/)
* class [Line](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
