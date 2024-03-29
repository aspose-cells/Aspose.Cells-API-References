---
title: Line
second_title: Aspose.Cells for .NET API 参考
description: 封装表示行格式的对象
type: docs
weight: 2200
url: /zh/net/aspose.cells.drawing/line/
---
## Line class

封装表示行格式的对象。

```csharp
public class Line
```

## 特性

| 姓名 | 描述 |
| --- | --- |
| [BeginArrowLength](../../aspose.cells.drawing/line/beginarrowlength) { get; set; } | 指定行首的箭头长度。 |
| [BeginArrowWidth](../../aspose.cells.drawing/line/beginarrowwidth) { get; set; } | 指定行首箭头的宽度。 |
| [BeginType](../../aspose.cells.drawing/line/begintype) { get; set; } | 指定行首的箭头。 |
| [CapType](../../aspose.cells.drawing/line/captype) { get; set; } | 指定结尾大写。 |
| [Color](../../aspose.cells.drawing/line/color) { get; set; } | 代表Color行的. |
| [CompoundType](../../aspose.cells.drawing/line/compoundtype) { get; set; } | 指定复合线型 |
| [DashType](../../aspose.cells.drawing/line/dashtype) { get; set; } | 指定虚线类型 |
| [EndArrowLength](../../aspose.cells.drawing/line/endarrowlength) { get; set; } | 指定行尾的箭头长度。 |
| [EndArrowWidth](../../aspose.cells.drawing/line/endarrowwidth) { get; set; } | 指定行尾的箭头宽度。 |
| [EndType](../../aspose.cells.drawing/line/endtype) { get; set; } | 指定行尾的箭头。 |
| [FormattingType](../../aspose.cells.drawing/line/formattingtype) { get; set; } | 获取或设置格式类型。 |
| [GradientFill](../../aspose.cells.drawing/line/gradientfill) { get; } | 表示渐变填充。 |
| [IsAuto](../../aspose.cells.drawing/line/isauto) { get; set; } | 指示此线型是否自动分配。 |
| [IsAutomaticColor](../../aspose.cells.drawing/line/isautomaticcolor) { get; } | 表示线的颜色是否自动分配。 |
| [IsVisible](../../aspose.cells.drawing/line/isvisible) { get; set; } | 表示线是否可见。 |
| [JoinType](../../aspose.cells.drawing/line/jointype) { get; set; } | 指定连接大写字母。 |
| [Style](../../aspose.cells.drawing/line/style) { get; set; } | 代表线条的样式。 |
| [ThemeColor](../../aspose.cells.drawing/line/themecolor) { get; set; } | 获取和设置主题颜色。 |
| [Transparency](../../aspose.cells.drawing/line/transparency) { get; set; } | 将线条的透明度返回或设置为从 0.0（不透明）到 1.0（透明）的值。 |
| [Weight](../../aspose.cells.drawing/line/weight) { get; set; } | 获取或设置[`WeightType`](../weighttype)行的. |
| [WeightPt](../../aspose.cells.drawing/line/weightpt) { get; set; } | 获取或设置线的权重，以点为单位。 |
| [WeightPx](../../aspose.cells.drawing/line/weightpx) { get; set; } | 获取或设置线条的权重，以像素为单位。 |

### 例子

```csharp

[C#]

Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];

Cells cells = sheet.Cells;
cells[0,1].PutValue("Income");
cells[1,0].PutValue("Company A");
cells[2,0].PutValue("Company B");
cells[3,0].PutValue("Company C");
cells[1,1].PutValue(10000);
cells[2,1].PutValue(20000);
cells[3,1].PutValue(30000);

int chartIndex = sheet.Charts.Add(ChartType.Line, 9, 9, 21, 15);
Chart chart = sheet.Charts[chartIndex];
//在 NSeries 的线条上应用虚线样式
chart.NSeries[0].Border.Style = LineType.Dot;
chart.NSeries[0].Border.Color = Color.Red;
//在 NSeries 的数据标记上应用三角形标记样式
chart.NSeries[0].Marker.MarkerStyle = ChartMarkerType.Triangle;
//将NSeries中所有行的权重设置为medium
chart.NSeries[0].Border.Weight = WeightType.MediumLine;

[Visual Basic]

Dim workbook as Workbook = new Workbook()
Dim sheet as Worksheet = workbook.Worksheets(0)

Dim cells as Cells = sheet.Cells
cells(0,1).PutValue("Income")
cells(1,0).PutValue("Company A")
cells(2,0).PutValue("Company B")
cells(3,0).PutValue("Company C")
cells(1,1).PutValue(10000)
cells(2,1).PutValue(20000)
cells(3,1).PutValue(30000)
		
Dim chartIndex as Integer = sheet.Charts.Add(ChartType.Column, 9, 9, 21, 15)    ///
Dim chart as Chart = sheet.Charts(chartIndex)
'在 NSeries 的线上应用虚线样式
chart.NSeries(0).Border.Style = LineType.Dot
chart.NSeries(0).Border.Color = Color.Red
'在 NSeries 的数据标记上应用三角形标记样式
chart.NSeries(0).Marker.MarkerStyle = ChartMarkerType.Triangle
'将 NSeries 中所有行的粗细设置为 medium
chart.NSeries(0).Border.Weight = WeightType.MediumLine
```

### 也可以看看

* 命名空间 [Aspose.Cells.Drawing](../../aspose.cells.drawing)
* 部件 [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
