##Line.BeginType
Line property. Specifies an arrowhead for the begin of a line
## Line.BeginType property
Specifies an arrowhead for the begin of a line.
```csharp
public MsoArrowheadStyle BeginType { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Charts;
using System.Drawing;
namespace AsposeCellsExamples
{
public class LinePropertyBeginTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue(10);
worksheet.Cells["A2"].PutValue(20);
worksheet.Cells["A3"].PutValue(30);
// Add a line chart
int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 15, 5);
Chart chart = worksheet.Charts[chartIndex];
// Set chart data source
chart.NSeries.Add("A1:A3", true);
// Get the first series and configure its line properties
Series series = chart.NSeries[0];
series.Border.BeginType = MsoArrowheadStyle.Arrow;
series.Border.EndType = MsoArrowheadStyle.ArrowDiamond;
series.Border.Color = Color.Red;
series.Border.Weight = WeightType.MediumLine;
// Save the workbook
workbook.Save("LinePropertyBeginTypeDemo.xlsx");
}
}
}
```
### See Also
* enum [MsoArrowheadStyle](../../msoarrowheadstyle/)
* class [Line](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
