---
title: FillFormat
second_title: Aspose.Cells for .NET API 参考
description: 封装表示形状填充格式的对象
type: docs
weight: 1970
url: /zh/net/aspose.cells.drawing/fillformat/
---
## FillFormat class

封装表示形状填充格式的对象。

```csharp
public class FillFormat
```

## 特性

| 姓名 | 描述 |
| --- | --- |
| [FillType](../../aspose.cells.drawing/fillformat/filltype) { get; set; } | 获取和设置填充类型 |
| [GradientColor1](../../aspose.cells.drawing/fillformat/gradientcolor1) { get; } | 返回指定填充的渐变颜色 1。 |
| [GradientColor2](../../aspose.cells.drawing/fillformat/gradientcolor2) { get; } | 返回指定填充的渐变颜色 2。 |
| [GradientColorType](../../aspose.cells.drawing/fillformat/gradientcolortype) { get; } | 返回指定填充的渐变颜色类型。 |
| [GradientDegree](../../aspose.cells.drawing/fillformat/gradientdegree) { get; } | 返回指定填充的渐变度。 仅适用于 Excel 2007。 |
| [GradientFill](../../aspose.cells.drawing/fillformat/gradientfill) { get; } | 获取[`GradientFill`](./gradientfill)对象. |
| [GradientStyle](../../aspose.cells.drawing/fillformat/gradientstyle) { get; } | 返回指定填充的渐变样式。 |
| [GradientVariant](../../aspose.cells.drawing/fillformat/gradientvariant) { get; } | 返回指定填充的渐变变量。 仅适用于 Excel 2007。 |
| [ImageData](../../aspose.cells.drawing/fillformat/imagedata) { get; set; } | 获取和设置图片图像数据。 |
| [Pattern](../../aspose.cells.drawing/fillformat/pattern) { get; set; } | 代表一个区域的显示模式。 |
| [PatternFill](../../aspose.cells.drawing/fillformat/patternfill) { get; } | 获取[`PatternFill`](./patternfill)对象. |
| [PictureFormatType](../../aspose.cells.drawing/fillformat/pictureformattype) { get; set; } | 获取和设置图片格式类型。 |
| [PresetColor](../../aspose.cells.drawing/fillformat/presetcolor) { get; } | 返回指定填充的渐变预设颜色。 |
| [Scale](../../aspose.cells.drawing/fillformat/scale) { get; set; } | 获取和设置图片格式比例。 |
| [SolidFill](../../aspose.cells.drawing/fillformat/solidfill) { get; } | 获取[`SolidFill`](./solidfill)对象. |
| [Texture](../../aspose.cells.drawing/fillformat/texture) { get; set; } | 表示指定填充的纹理类型。 |
| [TextureFill](../../aspose.cells.drawing/fillformat/texturefill) { get; } | 获取[`TextureFill`](./texturefill)对象. |
| [Transparency](../../aspose.cells.drawing/fillformat/transparency) { get; set; } | 将区域的透明度返回或设置为从 0.0（不透明）到 1.0（透明）的值。 |

## 方法

| 姓名 | 描述 |
| --- | --- |
| override [Equals](../../aspose.cells.drawing/fillformat/equals)(object) |  |
| override [GetHashCode](../../aspose.cells.drawing/fillformat/gethashcode)() | 获取哈希码。 |
| [SetOneColorGradient](../../aspose.cells.drawing/fillformat/setonecolorgradient)(Color, double, GradientStyleType, int) | 将指定的填充设置为单色渐变。 仅适用于 Excel 2007。 |
| [SetPresetColorGradient](../../aspose.cells.drawing/fillformat/setpresetcolorgradient)(GradientPresetType, GradientStyleType, int) | 将指定的填充设置为预设颜色渐变。 仅适用于 Excel 2007。 |
| [SetTwoColorGradient](../../aspose.cells.drawing/fillformat/settwocolorgradient#settwocolorgradient_1)(Color, Color, GradientStyleType, int) | 将指定的填充设置为双色渐变。 仅适用于 Excel 2007。 |
| [SetTwoColorGradient](../../aspose.cells.drawing/fillformat/settwocolorgradient#settwocolorgradient)(Color, double, Color, double, GradientStyleType, int) | 将指定的填充设置为双色渐变。 仅适用于 Excel 2007。 |

### 例子

```csharp

[C#]

//实例化一个工作簿对象
Workbook workbook = new Workbook();
//向Excel对象添加一个新的工作表
int sheetIndex = workbook.Worksheets.Add();
//通过传入工作表的索引来获取新添加的工作表的引用
Worksheet worksheet = workbook.Worksheets[sheetIndex];
//向“A1”单元格添加样本值
worksheet.Cells["A1"].PutValue(50);
//向“A2”单元格添加样本值
worksheet.Cells["A2"].PutValue(100);
//向“A3”单元格添加样本值
worksheet.Cells["A3"].PutValue(150);
//向“A4”单元格添加样本值
worksheet.Cells["A4"].PutValue(200);
//向“B1”单元格添加样本值
worksheet.Cells["B1"].PutValue(60);
//向“B2”单元格添加样本值
worksheet.Cells["B2"].PutValue(32);
//向“B3”单元格添加样本值
worksheet.Cells["B3"].PutValue(50);
//向“B4”单元格添加样本值
worksheet.Cells["B4"].PutValue(40);
//将样本值添加到“C1”单元格作为类别数据
worksheet.Cells["C1"].PutValue("Q1");
//将样本值添加到“C2”单元格作为类别数据
worksheet.Cells["C2"].PutValue("Q2");
//将样本值添加到“C3”单元格作为类别数据
worksheet.Cells["C3"].PutValue("Y1");
//将样本值添加到“C4”单元格作为类别数据
worksheet.Cells["C4"].PutValue("Y2");
//向工作表添加图表
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
//访问新添加图表的实例
Chart chart = worksheet.Charts[chartIndex];
//将NSeries（图表数据源）添加到从“A1”单元格到“B4”单元格的图表中
int seriesIndex = chart.NSeries.Add("A1:B4", true);
//设置NSeries类别数据的数据源
chart.NSeries.CategoryData = "C1:C4";
//用渐变填充第二个NSeries的区域
chart.NSeries[seriesIndex].Area.FillFormat.SetOneColorGradient(Color.Lime, 1, GradientStyleType.Horizontal, 1);

[Visual Basic]

实例化工作簿对象
Dim workbook As Workbook = New Workbook()
'向 Excel 对象添加新工作表
Dim sheetIndex As Int32 = workbook.Worksheets.Add()
'通过传入工作表的索引来获取新添加的工作表的引用
Dim worksheet As Worksheet = workbook.Worksheets(sheetIndex)
'Adding a sample value to "A1" cell
worksheet.Cells("A1").PutValue(50)
'Adding a sample value to "A2" cell
worksheet.Cells("A2").PutValue(100)
'Adding a sample value to "A3" cell
worksheet.Cells("A3").PutValue(150)
'Adding a sample value to "A4" cell
worksheet.Cells("A4").PutValue(200)
'Adding a sample value to "B1" cell
worksheet.Cells("B1").PutValue(60)
'Adding a sample value to "B2" cell
worksheet.Cells("B2").PutValue(32)
'Adding a sample value to "B3" cell
worksheet.Cells("B3").PutValue(50)
'Adding a sample value to "B4" cell
worksheet.Cells("B4").PutValue(40)
'Adding a sample value to "C1" cell as category data
worksheet.Cells("C1").PutValue("Q1")
'Adding a sample value to "C2" cell as category data
worksheet.Cells("C2").PutValue("Q2")
'Adding a sample value to "C3" cell as category data
worksheet.Cells("C3").PutValue("Y1")
'Adding a sample value to "C4" cell as category data
worksheet.Cells("C4").PutValue("Y2")
'将图表添加到工作表
Dim chartIndex As Int32 = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5)
'访问新添加图表的实例
Dim chart As Chart = worksheet.Charts(chartIndex)
'Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B4"
Dim seriesIndex As Int32 = chart.NSeries.Add("A1:B4", True)
'设置 NSeries 类别数据的数据源
chart.NSeries.CategoryData = "C1:C4"
'用渐变填充第二个 NSeries 的区域
chart.NSeries(seriesIndex).Area.FillFormat.SetOneColorGradient(Color.Lime, 1, GradientStyleType.Horizontal, 1)
```

### 也可以看看

* 命名空间 [Aspose.Cells.Drawing](../../aspose.cells.drawing)
* 部件 [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
