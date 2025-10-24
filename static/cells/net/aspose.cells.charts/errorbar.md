##Class ErrorBar
Aspose.Cells.Charts.ErrorBar class. Represents error bar of data series
## ErrorBar class
Represents error bar of data series.
```csharp
public class ErrorBar : Line
```
## Properties
| Name | Description |
| --- | --- |
| [Amount](../../aspose.cells.charts/errorbar/amount/) { get; set; } | Represents amount of error bar. |
| [BeginArrowLength](../../aspose.cells.drawing/line/beginarrowlength/) { get; set; } | Specifies the length of the arrowhead for the begin of a line.(Inherited from [`Line`](../../aspose.cells.drawing/line/).) |
| [BeginArrowWidth](../../aspose.cells.drawing/line/beginarrowwidth/) { get; set; } | Specifies the width of the arrowhead for the begin of a line.(Inherited from [`Line`](../../aspose.cells.drawing/line/).) |
| [BeginType](../../aspose.cells.drawing/line/begintype/) { get; set; } | Specifies an arrowhead for the begin of a line.(Inherited from [`Line`](../../aspose.cells.drawing/line/).) |
| [CapType](../../aspose.cells.drawing/line/captype/) { get; set; } | Specifies the ending caps.(Inherited from [`Line`](../../aspose.cells.drawing/line/).) |
| [Color](../../aspose.cells.drawing/line/color/) { get; set; } | Represents the Color of the line.(Inherited from [`Line`](../../aspose.cells.drawing/line/).) |
| [CompoundType](../../aspose.cells.drawing/line/compoundtype/) { get; set; } | Specifies the compound line type(Inherited from [`Line`](../../aspose.cells.drawing/line/).) |
| [DashType](../../aspose.cells.drawing/line/dashtype/) { get; set; } | Specifies the dash line type(Inherited from [`Line`](../../aspose.cells.drawing/line/).) |
| [DisplayType](../../aspose.cells.charts/errorbar/displaytype/) { get; set; } | Represents the display type of error bar. |
| [EndArrowLength](../../aspose.cells.drawing/line/endarrowlength/) { get; set; } | Specifies the length of the arrowhead for the end of a line.(Inherited from [`Line`](../../aspose.cells.drawing/line/).) |
| [EndArrowWidth](../../aspose.cells.drawing/line/endarrowwidth/) { get; set; } | Specifies the width of the arrowhead for the end of a line.(Inherited from [`Line`](../../aspose.cells.drawing/line/).) |
| [EndType](../../aspose.cells.drawing/line/endtype/) { get; set; } | Specifies an arrowhead for the end of a line.(Inherited from [`Line`](../../aspose.cells.drawing/line/).) |
| [FormattingType](../../aspose.cells.drawing/line/formattingtype/) { get; set; } | Gets or sets format type.(Inherited from [`Line`](../../aspose.cells.drawing/line/).) |
| [GradientFill](../../aspose.cells.drawing/line/gradientfill/) { get; } | Represents gradient fill.(Inherited from [`Line`](../../aspose.cells.drawing/line/).) |
| [IsAuto](../../aspose.cells.drawing/line/isauto/) { get; set; } | Indicates whether this line style is auto assigned.(Inherited from [`Line`](../../aspose.cells.drawing/line/).) |
| [IsAutomaticColor](../../aspose.cells.drawing/line/isautomaticcolor/) { get; } | Indicates whether the color of line is automatic assigned.(Inherited from [`Line`](../../aspose.cells.drawing/line/).) |
| [IsVisible](../../aspose.cells.drawing/line/isvisible/) { get; set; } | Represents whether the line is visible.(Inherited from [`Line`](../../aspose.cells.drawing/line/).) |
| [JoinType](../../aspose.cells.drawing/line/jointype/) { get; set; } | Specifies the joining caps.(Inherited from [`Line`](../../aspose.cells.drawing/line/).) |
| [MinusValue](../../aspose.cells.charts/errorbar/minusvalue/) { get; set; } | Represents negative error amount when error bar type is Custom. |
| [PlusValue](../../aspose.cells.charts/errorbar/plusvalue/) { get; set; } | Represents positive error amount when error bar type is Custom. |
| [ShowMarkerTTop](../../aspose.cells.charts/errorbar/showmarkerttop/) { get; set; } | Indicates if formatting error bars with a T-top. |
| [Style](../../aspose.cells.drawing/line/style/) { get; set; } | Represents the style of the line.(Inherited from [`Line`](../../aspose.cells.drawing/line/).) |
| [ThemeColor](../../aspose.cells.drawing/line/themecolor/) { get; set; } | Gets and sets the theme color.(Inherited from [`Line`](../../aspose.cells.drawing/line/).) |
| [Transparency](../../aspose.cells.drawing/line/transparency/) { get; set; } | Returns or sets the degree of transparency of the line as a value from 0.0 (opaque) through 1.0 (clear).(Inherited from [`Line`](../../aspose.cells.drawing/line/).) |
| [Type](../../aspose.cells.charts/errorbar/type/) { get; set; } | Represents error bar amount type. |
| [Weight](../../aspose.cells.drawing/line/weight/) { get; set; } | Gets or sets the [`WeightType`](../../aspose.cells.drawing/weighttype/) of the line.(Inherited from [`Line`](../../aspose.cells.drawing/line/).) |
| [WeightPt](../../aspose.cells.drawing/line/weightpt/) { get; set; } | Gets or sets the weight of the line in unit of points.(Inherited from [`Line`](../../aspose.cells.drawing/line/).) |
| [WeightPx](../../aspose.cells.drawing/line/weightpx/) { get; set; } | Gets or sets the weight of the line in unit of pixels.(Inherited from [`Line`](../../aspose.cells.drawing/line/).) |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using System;
public class ErrorBarDemo
{
public static void ErrorBarExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
Cells cells = workbook.Worksheets[0].Cells;
// Add sample data to cells
cells["A1"].PutValue(2);
cells["A2"].PutValue(5);
cells["A3"].PutValue(3);
cells["A4"].PutValue(6);
cells["B1"].PutValue(4);
cells["B2"].PutValue(3);
cells["B3"].PutValue(6);
cells["B4"].PutValue(7);
cells["C1"].PutValue("Q1");
cells["C2"].PutValue("Q2");
cells["C3"].PutValue("Y1");
cells["C4"].PutValue("Y2");
// Add a chart to the worksheet
int chartIndex = workbook.Worksheets[0].Charts.Add(ChartType.Column, 11, 0, 27, 10);
Chart chart = workbook.Worksheets[0].Charts[chartIndex];
// Add NSeries (chart data source) to the chart
chart.NSeries.Add("A1:B4", true);
chart.NSeries.CategoryData = "C1:C4";
// Configure error bars for each series in the chart
for (int i = 0; i < chart.NSeries.Count; i++)
{
Series series = chart.NSeries[i];
series.YErrorBar.DisplayType = ErrorBarDisplayType.Minus;
series.YErrorBar.Type = ErrorBarType.FixedValue;
series.YErrorBar.Amount = 5;
// Additional properties for demonstration
series.YErrorBar.ShowMarkerTTop = true;
series.YErrorBar.PlusValue = "=Sheet1!A1";
series.YErrorBar.MinusValue = "=Sheet1!A2";
series.YErrorBar.CompoundType = Aspose.Cells.Drawing.MsoLineStyle.ThickThin;
series.YErrorBar.DashType = Aspose.Cells.Drawing.MsoLineDashStyle.DashDot;
series.YErrorBar.CapType = Aspose.Cells.Drawing.LineCapType.Round;
series.YErrorBar.JoinType = Aspose.Cells.Drawing.LineJoinType.Bevel;
series.YErrorBar.BeginType = Aspose.Cells.Drawing.MsoArrowheadStyle.Arrow;
series.YErrorBar.EndType = Aspose.Cells.Drawing.MsoArrowheadStyle.ArrowDiamond;
series.YErrorBar.BeginArrowLength = Aspose.Cells.Drawing.MsoArrowheadLength.Short;
series.YErrorBar.EndArrowLength = Aspose.Cells.Drawing.MsoArrowheadLength.Long;
series.YErrorBar.BeginArrowWidth = Aspose.Cells.Drawing.MsoArrowheadWidth.Narrow;
series.YErrorBar.EndArrowWidth = Aspose.Cells.Drawing.MsoArrowheadWidth.Wide;
series.YErrorBar.ThemeColor = new Aspose.Cells.ThemeColor(Aspose.Cells.ThemeColorType.Accent1, 0.5);
series.YErrorBar.Color = System.Drawing.Color.Red;
series.YErrorBar.Transparency = 0.5;
series.YErrorBar.Style = Aspose.Cells.Drawing.LineType.DashDotDot;
series.YErrorBar.Weight = Aspose.Cells.Drawing.WeightType.WideLine;
series.YErrorBar.WeightPt = 2.0;
series.YErrorBar.WeightPx = 3.0;
series.YErrorBar.FormattingType = ChartLineFormattingType.Gradient;
series.YErrorBar.IsVisible = true;
series.YErrorBar.IsAuto = false;
}
// Save the workbook
workbook.Save("ErrorBarExample.xlsx");
workbook.Save("ErrorBarExample.pdf");
}
}
}
```
### See Also
* class [Line](../../aspose.cells.drawing/line/)
* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)
