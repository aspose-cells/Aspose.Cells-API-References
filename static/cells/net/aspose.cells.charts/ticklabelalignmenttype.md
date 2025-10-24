##Enum TickLabelAlignmentType
Aspose.Cells.Charts.TickLabelAlignmentType enum. Represents the text alignment type for the tick labels on the axis
## TickLabelAlignmentType enumeration
Represents the text alignment type for the tick labels on the axis
```csharp
public enum TickLabelAlignmentType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Center | `0` | Represents the text shall be centered. |
| Left | `1` | Represents the text shall be left justified. |
| Right | `2` | Represents the text shall be right justified. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using System;
public class TickLabelAlignmentTypeDemo
{
public static void TickLabelAlignmentTypeExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for the chart
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
// Add series to the chart
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
// Access the tick labels of the category axis
TickLabels tickLabels = chart.CategoryAxis.TickLabels;
// Set the alignment type for the tick labels
tickLabels.AlignmentType = TickLabelAlignmentType.Center;
// Save the workbook
workbook.Save("TickLabelAlignmentTypeExample.xlsx");
return;
}
}
}
```
### See Also
* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)
