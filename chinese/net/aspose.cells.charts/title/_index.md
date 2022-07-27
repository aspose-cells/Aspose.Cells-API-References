---
title: Title
second_title: Aspose.Cells for .NET API 参考
description: 封装表示图表或轴标题的对象
type: docs
weight: 970
url: /zh/net/aspose.cells.charts/title/
---
## Title class

封装表示图表或轴标题的对象。

```csharp
public class Title : ChartTextFrame
```

## 特性

| 姓名 | 描述 |
| --- | --- |
| virtual [Area](../../aspose.cells.charts/chartframe/area) { get; } | 获取[`区域`](../chartframe/area). |
| virtual [AutoScaleFont](../../aspose.cells.charts/chartframe/autoscalefont) { get; set; } | 如果对象中的文本在对象大小更改时更改字体大小，则为真。默认值是true。 |
| [BackgroundMode](../../aspose.cells.charts/chartframe/backgroundmode) { get; set; } | 获取和设置背景的显示模式 |
| virtual [Border](../../aspose.cells.charts/chartframe/border) { get; } | 获取[`边界`](../../aspose.cells.drawing/line). |
| [DefaultHeight](../../aspose.cells.charts/chartframe/defaultheight) { get; } | 表示默认位置的高度 |
| [DefaultWidth](../../aspose.cells.charts/chartframe/defaultwidth) { get; } | 表示默认位置的宽度 |
| [DefaultX](../../aspose.cells.charts/chartframe/defaultx) { get; } | 代表默认位置的 x |
| [DefaultY](../../aspose.cells.charts/chartframe/defaulty) { get; } | 代表默认位置的y |
| virtual [DirectionType](../../aspose.cells.charts/charttextframe/directiontype) { get; set; } | 获取和设置文本的方向。 |
| virtual [Font](../../aspose.cells.charts/chartframe/font) { get; } | 得到一个[`Font`](../chartframe/font)指定 ChartFrame 对象的对象。 |
| virtual [Height](../../aspose.cells.charts/chartframe/height) { get; set; } | 获取或设置边框高度，单位为图表区域的1/4000。 |
| virtual [IsAutomaticSize](../../aspose.cells.charts/chartframe/isautomaticsize) { get; set; } | 指示图表框是否自动调整大小。 |
| virtual [IsAutoText](../../aspose.cells.charts/charttextframe/isautotext) { get; set; } | 表示文本是自动生成的。 |
| [IsDefaultPosBeSet](../../aspose.cells.charts/chartframe/isdefaultposbeset) { get; } | 表示是否设置了默认位置（DefaultX、DefaultY、DefaultWidth 和 DefaultHeight）。 |
| [IsDeleted](../../aspose.cells.charts/charttextframe/isdeleted) { get; set; } | 表示此数据标签是否被删除。 |
| [IsInnerMode](../../aspose.cells.charts/chartframe/isinnermode) { get; set; } | 表示绘图区域大小的大小是否包含刻度线和轴标签。 False 指定大小应确定绘图区域的大小、刻度线和轴标签。 |
| [IsResizeShapeToFitText](../../aspose.cells.charts/charttextframe/isresizeshapetofittext) { get; set; } | 获取或设置一个形状是否应该自动适应以完全包含其中描述的文本。当形状内的文本被缩放以包含其中的所有文本时，自动拟合 is 。 |
| virtual [IsTextWrapped](../../aspose.cells.charts/charttextframe/istextwrapped) { get; set; } | 获取或设置一个值，该值指示文本是否被换行。 |
| [IsVisible](../../aspose.cells.charts/title/isvisible) { get; set; } | 表示标题是否可见。 |
| virtual [LinkedSource](../../aspose.cells.charts/charttextframe/linkedsource) { get; set; } | 获取并设置对工作表的引用。 |
| [OverLay](../../aspose.cells.charts/title/overlay) { get; set; } | 表示图表上的覆盖居中标题而不调整图表大小。 |
| [ReadingOrder](../../aspose.cells.charts/charttextframe/readingorder) { get; set; } | 代表文字阅读顺序。 |
| [RotationAngle](../../aspose.cells.charts/charttextframe/rotationangle) { get; set; } | 代表文字旋转角度。 |
| [Shadow](../../aspose.cells.charts/chartframe/shadow) { get; set; } | 如果框架有阴影则为真。 |
| [ShapeProperties](../../aspose.cells.charts/chartframe/shapeproperties) { get; } | 获取[`ShapeProperties`](../chartframe/shapeproperties)对象. |
| override [Text](../../aspose.cells.charts/title/text) { get; set; } | 获取或设置显示单元标签的文本。 |
| [TextHorizontalAlignment](../../aspose.cells.charts/charttextframe/texthorizontalalignment) { get; set; } | 获取和设置文本水平对齐方式。 |
| [TextVerticalAlignment](../../aspose.cells.charts/charttextframe/textverticalalignment) { get; set; } | 获取或设置文本的文本垂直对齐方式。 |
| virtual [Width](../../aspose.cells.charts/chartframe/width) { get; set; } | 获取或设置边框宽度，以图表区域的 1/4000 为单位。 |
| override [X](../../aspose.cells.charts/title/x) { get; set; } | 获取或设置左上角的x坐标，单位为图表区域的1/4000。 |
| override [Y](../../aspose.cells.charts/title/y) { get; set; } | 获取或设置左上角的y坐标，单位为图表区域的1/4000。 |

## 方法

| 姓名 | 描述 |
| --- | --- |
| [Characters](../../aspose.cells.charts/title/characters#characters_1)() | 获取此标题的富文本格式。 |
| [Characters](../../aspose.cells.charts/charttextframe/characters)(int, int) | 返回一个 Characters 对象，该对象表示文本中的一系列字符。 |
| virtual [SetPositionAuto](../../aspose.cells.charts/chartframe/setpositionauto)() | 将框架的位置设置为自动 |

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
		
int chartIndex = sheet.Charts.Add(ChartType.Column, 9, 9, 21, 15);
Chart chart = sheet.Charts[chartIndex];

//设置图表的标题
chart.Title.Text = "Title";
//设置图表标题的字体颜色为蓝色
chart.Title.Font.Color = Color.Blue;
//设置图表类别轴的标题
chart.CategoryAxis.Title.Text = "Category";
//设置图表数值轴的标题
chart.ValueAxis.Title.Text = "Value";

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

'设置图表的标题
chart.Title.Text = "Title"
'将图表标题的字体颜色设置为蓝色
chart.Title.Font.Color = Color.Blue
'设置图表类别轴的标题
chart.CategoryAxis.Title.Text = "Category"
'设置图表数值轴的标题
chart.ValueAxis.Title.Text = "Value"

```

### 也可以看看

* class [ChartTextFrame](../charttextframe)
* 命名空间 [Aspose.Cells.Charts](../../aspose.cells.charts)
* 部件 [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
