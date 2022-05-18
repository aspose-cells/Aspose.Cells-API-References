---
title: ErrorBar
second_title: Aspose.Cells for .NET API Reference
description: 
type: docs
weight: 620
url: /net/aspose.cells.charts/errorbar/
---
## ErrorBar class

Represents error bar of data series.

```csharp
public class ErrorBar : Line
```

## Properties

| Name | Description |
| --- | --- |
| [Amount](../../aspose.cells.charts/errorbar/amount) { get; set; } | Represents amount of error bar.  The amount must be greater than and equal to zero. |
| [BeginArrowLength](../../aspose.cells.drawing/line/beginarrowlength) { get; set; } | Specifies the length of the arrowhead for the begin of a line. |
| [BeginArrowWidth](../../aspose.cells.drawing/line/beginarrowwidth) { get; set; } | Specifies the width of the arrowhead for the begin of a line. |
| [BeginType](../../aspose.cells.drawing/line/begintype) { get; set; } | Specifies an arrowhead for the begin of a line. |
| [CapType](../../aspose.cells.drawing/line/captype) { get; set; } | Specifies the ending caps. |
| [Color](../../aspose.cells.drawing/line/color) { get; set; } | Represents the Color of the line. |
| [CompoundType](../../aspose.cells.drawing/line/compoundtype) { get; set; } | Specifies the compound line type |
| [DashType](../../aspose.cells.drawing/line/dashtype) { get; set; } | Specifies the dash line type |
| [DisplayType](../../aspose.cells.charts/errorbar/displaytype) { get; set; } | Represents error bar display type. |
| [EndArrowLength](../../aspose.cells.drawing/line/endarrowlength) { get; set; } | Specifies the length of the arrowhead for the end of a line. |
| [EndArrowWidth](../../aspose.cells.drawing/line/endarrowwidth) { get; set; } | Specifies the width of the arrowhead for the end of a line. |
| [EndType](../../aspose.cells.drawing/line/endtype) { get; set; } | Specifies an arrowhead for the end of a line. |
| [FormattingType](../../aspose.cells.drawing/line/formattingtype) { get; set; } | Gets or sets format type. |
| [GradientFill](../../aspose.cells.drawing/line/gradientfill) { get; } | Represents gradient fill. |
| [IsAuto](../../aspose.cells.drawing/line/isauto) { get; set; } | Indicates whether this line style is auto assigned. |
| [IsAutomaticColor](../../aspose.cells.drawing/line/isautomaticcolor) { get; } | Indicates whether the color of line is automatic assigned. |
| [IsVisible](../../aspose.cells.drawing/line/isvisible) { get; set; } | Represents whether the line is visible. |
| [JoinType](../../aspose.cells.drawing/line/jointype) { get; set; } | Specifies the joining caps. |
| [MinusValue](../../aspose.cells.charts/errorbar/minusvalue) { get; set; } | Represents negative error amount when error bar type is Custom. |
| [PlusValue](../../aspose.cells.charts/errorbar/plusvalue) { get; set; } | Represents positive error amount when error bar type is Custom. |
| [ShowMarkerTTop](../../aspose.cells.charts/errorbar/showmarkerttop) { get; set; } | Indicates if formatting error bars with a T-top. |
| [Style](../../aspose.cells.drawing/line/style) { get; set; } | Represents the style of the line. |
| [ThemeColor](../../aspose.cells.drawing/line/themecolor) { get; set; } | Gets and sets the theme color. |
| [Transparency](../../aspose.cells.drawing/line/transparency) { get; set; } | Returns or sets the degree of transparency of the line as a value from 0.0 (opaque) through 1.0 (clear). |
| [Type](../../aspose.cells.charts/errorbar/type) { get; set; } | Represents error bar amount type. |
| [Weight](../../aspose.cells.drawing/line/weight) { get; set; } | Gets or sets the [`WeightType`](../../aspose.cells.drawing/weighttype) of the line. |
| [WeightPt](../../aspose.cells.drawing/line/weightpt) { get; set; } | Gets or sets the weight of the line in unit of points. |
| [WeightPx](../../aspose.cells.drawing/line/weightpx) { get; set; } | Gets or sets the weight of the line in unit of pixels. |

### Examples

```csharp
[C#]
Workbook workbook = new Workbook();
Cells cells = workbook.Worksheets[0].Cells;
cells["a1"].PutValue(2);
cells["a2"].PutValue(5);
cells["a3"].PutValue(3);
cells["a4"].PutValue(6);
cells["b1"].PutValue(4);
cells["b2"].PutValue(3);
cells["b3"].PutValue(6);
cells["b4"].PutValue(7);

cells["C1"].PutValue("Q1");
cells["C2"].PutValue("Q2");
cells["C3"].PutValue("Y1");
cells["C4"].PutValue("Y2");

int chartIndex = excel.Worksheets[0].Charts.Add(ChartType.Column, 11, 0, 27, 10);

Chart chart = excel.Worksheets[0].Charts[chartIndex];
chart.NSeries.Add("A1:B4", true);

chart.NSeries.CategoryData = "C1:C4";

for(int i = 0; i < chart.NSeries.Count; i ++)
{
	ASeries aseries = chart.NSeries[i];
	aseries.YErrorBar.DisplayType = ErrorBarDisplayType.Minus;
	aseries.YErrorBar.Type = ErrorBarType.FixedValue;
	aseries.YErrorBar.Amount = 5;
}

[Visual Basic]
Dim workbook As Workbook =  New Workbook() 
Dim cells As Cells =  workbook.Worksheets(0).Cells 
cells("a1").PutValue(2)
cells("a2").PutValue(5)
cells("a3").PutValue(3)
cells("a4").PutValue(6)
cells("b1").PutValue(4)
cells("b2").PutValue(3)
cells("b3").PutValue(6)
cells("b4").PutValue(7)

cells("C1").PutValue("Q1")
cells("C2").PutValue("Q2")
cells("C3").PutValue("Y1")
cells("C4").PutValue("Y2")

Dim chartIndex As Integer =  excel.Worksheets(0).Charts.Add(ChartType.Column,11,0,27,10) 

Dim chart As Chart =  excel.Worksheets(0).Charts(chartIndex) 
chart.NSeries.Add("A1:B4", True)

chart.NSeries.CategoryData = "C1:C4"

Dim i As Integer
For  i = 0 To chart.NSeries.Count - 1
Dim aseries As ASeries =  chart.NSeries(i) 
aseries.YErrorBar.DisplayType = ErrorBarDisplayType.Minus
aseries.YErrorBar.Type = ErrorBarType.FixedValue
aseries.YErrorBar.Amount = 5
Next
```

### See Also

* class [Line](../../aspose.cells.drawing/line)
* namespace [Aspose.Cells.Charts](../../aspose.cells.charts)
* assembly [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
