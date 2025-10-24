##Class TickLabels
Aspose.Cells.Charts.TickLabels class. Represents the tickmark labels associated with tick marks on a chart axis
## TickLabels class
Represents the tick-mark labels associated with tick marks on a chart axis.
```csharp
public class TickLabels
```
## Properties
| Name | Description |
| --- | --- |
| [AlignmentType](../../aspose.cells.charts/ticklabels/alignmenttype/) { get; set; } | Gets and sets the text alignment for the tick labels on the axis. |
| [AutoScaleFont](../../aspose.cells.charts/ticklabels/autoscalefont/) { get; set; } | True if the text in the object changes font size when the object size changes. The default value is True. |
| [BackgroundMode](../../aspose.cells.charts/ticklabels/backgroundmode/) { get; set; } | Gets and sets the display mode of the background |
| [DirectionType](../../aspose.cells.charts/ticklabels/directiontype/) { get; set; } | Gets and sets the direction of text. |
| [DisplayNumberFormat](../../aspose.cells.charts/ticklabels/displaynumberformat/) { get; } | Gets and sets the display number format of tick labels. |
| [Font](../../aspose.cells.charts/ticklabels/font/) { get; } | Returns a [`Font`](./font/) object that represents the font of the specified TickLabels object. |
| [IsAutomaticRotation](../../aspose.cells.charts/ticklabels/isautomaticrotation/) { get; set; } | Indicates whether the rotation angle is automatic |
| [Number](../../aspose.cells.charts/ticklabels/number/) { get; set; } | Represents the format number for the TickLabels object. |
| [NumberFormat](../../aspose.cells.charts/ticklabels/numberformat/) { get; set; } | Represents the format string for the TickLabels object. |
| [NumberFormatLinked](../../aspose.cells.charts/ticklabels/numberformatlinked/) { get; set; } | True if the number format is linked to the cells (so that the number format changes in the labels when it changes in the cells). |
| [Offset](../../aspose.cells.charts/ticklabels/offset/) { get; set; } | Gets and sets the distance of labels from the category axis. Only for category (x) axis. |
| [ReadingOrder](../../aspose.cells.charts/ticklabels/readingorder/) { get; set; } | Represents text reading order. |
| [RotationAngle](../../aspose.cells.charts/ticklabels/rotationangle/) { get; set; } | Represents text rotation angle in clockwise. |
| [TextDirection](../../aspose.cells.charts/ticklabels/textdirection/) { get; set; } | (**Obsolete.**) Represents text reading order. |
| [TickLabelItems](../../aspose.cells.charts/ticklabels/ticklabelitems/) { get; } | Gets the display tick labels of the axis. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using System;
public class TickLabelsDemo
{
public static void TickLabelsExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for the chart
worksheet.Cells["A1"].PutValue(50);
worksheet.Cells["A2"].PutValue(100);
worksheet.Cells["A3"].PutValue(150);
worksheet.Cells["B1"].PutValue(4);
worksheet.Cells["B2"].PutValue(20);
worksheet.Cells["B3"].PutValue(50);
// Add a chart to the worksheet
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 25, 5);
Chart chart = worksheet.Charts[chartIndex];
// Add NSeries (chart data source) to the chart ranging from "A1" cell to "B3"
chart.NSeries.Add("A1:B3", true);
// Access the value axis
Axis valueAxis = chart.ValueAxis;
// Access the tick labels of the value axis
TickLabels tickLabels = valueAxis.TickLabels;
// Set properties of the tick labels
tickLabels.AutoScaleFont = true;
tickLabels.BackgroundMode = BackgroundMode.Transparent;
tickLabels.RotationAngle = 45;
tickLabels.IsAutomaticRotation = false;
tickLabels.NumberFormat = "0.00";
tickLabels.Number = 2;
tickLabels.NumberFormatLinked = true;
tickLabels.Offset = 100;
tickLabels.TextDirection = TextDirectionType.LeftToRight;
tickLabels.ReadingOrder = TextDirectionType.LeftToRight;
tickLabels.DirectionType = ChartTextDirectionType.Horizontal;
tickLabels.AlignmentType = TickLabelAlignmentType.Center;
// Save the workbook
workbook.Save("TickLabelsExample.xlsx");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)
