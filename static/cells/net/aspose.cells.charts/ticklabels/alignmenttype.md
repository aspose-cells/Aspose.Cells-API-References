##TickLabels.AlignmentType
TickLabels property. Gets and sets the text alignment for the tick labels on the axis
## TickLabels.AlignmentType property
Gets and sets the text alignment for the tick labels on the axis.
```csharp
public TickLabelAlignmentType AlignmentType { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class TickLabelsPropertyAlignmentTypeDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["A2"].PutValue("A");
worksheet.Cells["A3"].PutValue("B");
worksheet.Cells["A4"].PutValue("C");
worksheet.Cells["B1"].PutValue("Value");
worksheet.Cells["B2"].PutValue(10);
worksheet.Cells["B3"].PutValue(20);
worksheet.Cells["B4"].PutValue(30);
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
Aspose.Cells.Charts.TickLabels tickLabels = chart.CategoryAxis.TickLabels;
tickLabels.AlignmentType = TickLabelAlignmentType.Center;
workbook.Save("TickLabelAlignmentTypeExample.xlsx");
}
}
}
```
### See Also
* enum [TickLabelAlignmentType](../../ticklabelalignmenttype/)
* class [TickLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
