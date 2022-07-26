---
title: DisplayUnitLabel
second_title: Aspose.Cells for .NET API 参考
description: 表示显示单元标签
type: docs
weight: 600
url: /zh/net/aspose.cells.charts/displayunitlabel/
---
## DisplayUnitLabel class

表示显示单元标签。

```csharp
public class DisplayUnitLabel : ChartTextFrame
```

## 特性

| 姓名 | 描述 |
| --- | --- |
| virtual [Area](../../aspose.cells.charts/chartframe/area) { get; } | 获取[`区域`](../chartframe/area). |
| override [AutoScaleFont](../../aspose.cells.charts/displayunitlabel/autoscalefont) { get; set; } | 如果对象中的文本在对象大小更改时更改字体大小，则为真。默认值是true。 |
| [BackgroundMode](../../aspose.cells.charts/chartframe/backgroundmode) { get; set; } | 获取和设置背景的显示模式 |
| virtual [Border](../../aspose.cells.charts/chartframe/border) { get; } | 获取[`边界`](../../aspose.cells.drawing/line). |
| [DefaultHeight](../../aspose.cells.charts/chartframe/defaultheight) { get; } | 表示默认位置的高度 |
| [DefaultWidth](../../aspose.cells.charts/chartframe/defaultwidth) { get; } | 表示默认位置的宽度 |
| [DefaultX](../../aspose.cells.charts/chartframe/defaultx) { get; } | 代表默认位置的 x |
| [DefaultY](../../aspose.cells.charts/chartframe/defaulty) { get; } | 代表默认位置的y |
| virtual [DirectionType](../../aspose.cells.charts/charttextframe/directiontype) { get; set; } | 获取和设置文本的方向。 |
| override [Font](../../aspose.cells.charts/displayunitlabel/font) { get; } | 得到一个[`Font`](./font)指定 ChartFrame 对象的对象。 |
| virtual [Height](../../aspose.cells.charts/chartframe/height) { get; set; } | 获取或设置边框高度，单位为图表区域的1/4000。 |
| virtual [IsAutomaticSize](../../aspose.cells.charts/chartframe/isautomaticsize) { get; set; } | 指示图表框是否自动调整大小。 |
| virtual [IsAutoText](../../aspose.cells.charts/charttextframe/isautotext) { get; set; } | 表示文本是自动生成的。 |
| [IsDefaultPosBeSet](../../aspose.cells.charts/chartframe/isdefaultposbeset) { get; } | 表示是否设置了默认位置（DefaultX、DefaultY、DefaultWidth 和 DefaultHeight）。 |
| [IsDeleted](../../aspose.cells.charts/charttextframe/isdeleted) { get; set; } | 表示此数据标签是否被删除。 |
| [IsInnerMode](../../aspose.cells.charts/chartframe/isinnermode) { get; set; } | 表示绘图区域大小的大小是否包含刻度线和轴标签。 False 指定大小应确定绘图区域的大小、刻度线和轴标签。 |
| [IsResizeShapeToFitText](../../aspose.cells.charts/charttextframe/isresizeshapetofittext) { get; set; } | 获取或设置一个形状是否应该自动适应以完全包含其中描述的文本。当形状内的文本被缩放以包含其中的所有文本时，自动拟合 is 。 |
| virtual [IsTextWrapped](../../aspose.cells.charts/charttextframe/istextwrapped) { get; set; } | 获取或设置一个值，该值指示文本是否被换行。 |
| virtual [LinkedSource](../../aspose.cells.charts/charttextframe/linkedsource) { get; set; } | 获取并设置对工作表的引用。 |
| [ReadingOrder](../../aspose.cells.charts/charttextframe/readingorder) { get; set; } | 代表文字阅读顺序。 |
| [RotationAngle](../../aspose.cells.charts/charttextframe/rotationangle) { get; set; } | 代表文字旋转角度。 |
| [Shadow](../../aspose.cells.charts/chartframe/shadow) { get; set; } | 如果框架有阴影则为真。 |
| [ShapeProperties](../../aspose.cells.charts/chartframe/shapeproperties) { get; } | 获取[`ShapeProperties`](../chartframe/shapeproperties)对象. |
| override [Text](../../aspose.cells.charts/displayunitlabel/text) { get; set; } | 获取或设置显示单元标签的文本。 |
| [TextHorizontalAlignment](../../aspose.cells.charts/charttextframe/texthorizontalalignment) { get; set; } | 获取和设置文本水平对齐方式。 |
| [TextVerticalAlignment](../../aspose.cells.charts/charttextframe/textverticalalignment) { get; set; } | 获取或设置文本的文本垂直对齐方式。 |
| virtual [Width](../../aspose.cells.charts/chartframe/width) { get; set; } | 获取或设置边框宽度，以图表区域的 1/4000 为单位。 |
| virtual [X](../../aspose.cells.charts/chartframe/x) { get; set; } | 获取或设置左上角的x坐标，单位为图表区域的1/4000。 |
| virtual [Y](../../aspose.cells.charts/chartframe/y) { get; set; } | 获取或设置左上角的y坐标，单位为图表区域的1/4000。 |

## 方法

| 姓名 | 描述 |
| --- | --- |
| [Characters](../../aspose.cells.charts/charttextframe/characters)(int, int) | 返回一个 Characters 对象，该对象表示文本中的一系列字符。 |
| virtual [SetPositionAuto](../../aspose.cells.charts/chartframe/setpositionauto)() | 将框架的位置设置为自动 |

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
chart.NSeries.Add("A1:B4", true);
//设置NSeries类别数据的数据源
chart.NSeries.CategoryData = "C1:C4";
//设置value(Y)轴的显示单位。
chart.ValueAxis.DisplayUnit = DisplayUnitType.Hundreds;
DisplayUnitLabel displayUnitLabel = chart.ValueAxis.DisplayUnitLabel;
//设置自定义显示单位标签
displayUnitLabel.Text = "100";
//保存Excel文件
workbook.Save("book1.xls");

[Visual Basic]

'实例化工作簿对象
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
chart.NSeries.Add("A1:B4", True)
'设置 NSeries 类别数据的数据源
Chart.NSeries.CategoryData = "C1:C4"
'设置数值（Y）轴的显示单位。
chart.ValueAxis.DisplayUnit = DisplayUnitType.Hundreds
Dim displayUnitLabel As DisplayUnitLabel = chart.ValueAxis.DisplayUnitLabel
'设置自定义显示单元标签
displayUnitLabel.Text = "100"
'保存 Excel 文件
workbook.Save("book1.xls")
```

### 也可以看看

* class [ChartTextFrame](../charttextframe)
* 命名空间 [Aspose.Cells.Charts](../../aspose.cells.charts)
* 部件 [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
