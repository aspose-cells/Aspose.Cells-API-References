---
title: ErrorBar
second_title: Aspose.Cells for .NET API 参考
description: 代表数据系列的误差条
type: docs
weight: 630
url: /zh/net/aspose.cells.charts/errorbar/
---
## ErrorBar class

代表数据系列的误差条。

```csharp
public class ErrorBar : Line
```

## 特性

| 姓名 | 描述 |
| --- | --- |
| [Amount](../../aspose.cells.charts/errorbar/amount) { get; set; } | 表示误差条的数量。 金额必须大于或等于零。 |
| [BeginArrowLength](../../aspose.cells.drawing/line/beginarrowlength) { get; set; } | 指定行首的箭头长度。 |
| [BeginArrowWidth](../../aspose.cells.drawing/line/beginarrowwidth) { get; set; } | 指定行首箭头的宽度。 |
| [BeginType](../../aspose.cells.drawing/line/begintype) { get; set; } | 指定行首的箭头。 |
| [CapType](../../aspose.cells.drawing/line/captype) { get; set; } | 指定结尾大写。 |
| [Color](../../aspose.cells.drawing/line/color) { get; set; } | 代表Color行的. |
| [CompoundType](../../aspose.cells.drawing/line/compoundtype) { get; set; } | 指定复合线型 |
| [DashType](../../aspose.cells.drawing/line/dashtype) { get; set; } | 指定虚线类型 |
| [DisplayType](../../aspose.cells.charts/errorbar/displaytype) { get; set; } | 表示误差条显示类型。 |
| [EndArrowLength](../../aspose.cells.drawing/line/endarrowlength) { get; set; } | 指定行尾的箭头长度。 |
| [EndArrowWidth](../../aspose.cells.drawing/line/endarrowwidth) { get; set; } | 指定行尾的箭头宽度。 |
| [EndType](../../aspose.cells.drawing/line/endtype) { get; set; } | 指定行尾的箭头。 |
| [FormattingType](../../aspose.cells.drawing/line/formattingtype) { get; set; } | 获取或设置格式类型。 |
| [GradientFill](../../aspose.cells.drawing/line/gradientfill) { get; } | 表示渐变填充。 |
| [IsAuto](../../aspose.cells.drawing/line/isauto) { get; set; } | 指示此线型是否自动分配。 |
| [IsAutomaticColor](../../aspose.cells.drawing/line/isautomaticcolor) { get; } | 表示线的颜色是否自动分配。 |
| [IsVisible](../../aspose.cells.drawing/line/isvisible) { get; set; } | 表示线是否可见。 |
| [JoinType](../../aspose.cells.drawing/line/jointype) { get; set; } | 指定连接大写字母。 |
| [MinusValue](../../aspose.cells.charts/errorbar/minusvalue) { get; set; } | 表示误差条类型为自定义时的负误差量。 |
| [PlusValue](../../aspose.cells.charts/errorbar/plusvalue) { get; set; } | 表示误差条类型为自定义时的正误差量。 |
| [ShowMarkerTTop](../../aspose.cells.charts/errorbar/showmarkerttop) { get; set; } | 指示是否使用 T-top 格式化错误栏。 |
| [Style](../../aspose.cells.drawing/line/style) { get; set; } | 代表线条的样式。 |
| [ThemeColor](../../aspose.cells.drawing/line/themecolor) { get; set; } | 获取和设置主题颜色。 |
| [Transparency](../../aspose.cells.drawing/line/transparency) { get; set; } | 将线条的透明度返回或设置为从 0.0（不透明）到 1.0（透明）的值。 |
| [Type](../../aspose.cells.charts/errorbar/type) { get; set; } | 表示误差条数量类型。 |
| [Weight](../../aspose.cells.drawing/line/weight) { get; set; } | 获取或设置[`WeightType`](../../aspose.cells.drawing/weighttype)行的. |
| [WeightPt](../../aspose.cells.drawing/line/weightpt) { get; set; } | 获取或设置线的权重，以点为单位。 |
| [WeightPx](../../aspose.cells.drawing/line/weightpx) { get; set; } | 获取或设置线条的权重，以像素为单位。 |

### 例子

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

### 也可以看看

* class [Line](../../aspose.cells.drawing/line)
* 命名空间 [Aspose.Cells.Charts](../../aspose.cells.charts)
* 部件 [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
