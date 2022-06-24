---
title: Legend
second_title: Aspose.Cells for .NET API 参考
description: 封装表示图表图例的对象
type: docs
weight: 690
url: /zh/net/aspose.cells.charts/legend/
---
## Legend class

封装表示图表图例的对象。

```csharp
public class Legend : ChartTextFrame
```

## 特性

| 姓名 | 描述 |
| --- | --- |
| virtual [Area](../../aspose.cells.charts/chartframe/area) { get; } | 获取[`区域`](../chartframe/area) 。 |
| virtual [AutoScaleFont](../../aspose.cells.charts/chartframe/autoscalefont) { get; set; } | 如果对象中的文本在对象大小更改时更改字体大小，则为真。默认值是true。 |
| [BackgroundMode](../../aspose.cells.charts/chartframe/backgroundmode) { get; set; } | 获取和设置背景的显示方式 |
| virtual [Border](../../aspose.cells.charts/chartframe/border) { get; } | 获取[`边框`](../../aspose.cells.drawing/line) 。 |
| [DefaultHeight](../../aspose.cells.charts/chartframe/defaultheight) { get; } | 表示默认位置的高度 |
| [DefaultWidth](../../aspose.cells.charts/chartframe/defaultwidth) { get; } | 表示默认位置的宽度 |
| [DefaultX](../../aspose.cells.charts/chartframe/defaultx) { get; } | 表示默认位置的 x |
| [DefaultY](../../aspose.cells.charts/chartframe/defaulty) { get; } | 代表默认位置的y |
| virtual [DirectionType](../../aspose.cells.charts/charttextframe/directiontype) { get; set; } | 获取和设置文本的方向。 |
| virtual [Font](../../aspose.cells.charts/chartframe/font) { get; } | 获取指定 ChartFrame 对象的[`Font`](../chartframe/font)对象。 |
| virtual [Height](../../aspose.cells.charts/chartframe/height) { get; set; } | 获取或设置框架高度，以图表区域的 1/4000 为单位。 |
| virtual [IsAutomaticSize](../../aspose.cells.charts/chartframe/isautomaticsize) { get; set; } | 指示图表框是否自动调整大小。 |
| virtual [IsAutoText](../../aspose.cells.charts/charttextframe/isautotext) { get; set; } | 表示文本是自动生成的。 |
| [IsDefaultPosBeSet](../../aspose.cells.charts/chartframe/isdefaultposbeset) { get; } | 表示是否设置了默认位置（DefaultX、DefaultY、DefaultWidth 和 DefaultHeight）。 |
| [IsDeleted](../../aspose.cells.charts/charttextframe/isdeleted) { get; set; } | 表示是否删除此数据标签。 |
| [IsInnerMode](../../aspose.cells.charts/chartframe/isinnermode) { get; set; } | 指示绘图区域大小的大小是否包括刻度线和轴标签。 False 指定大小应确定绘图区域、刻度线和轴标签的大小。 |
| [IsOverLay](../../aspose.cells.charts/legend/isoverlay) { get; set; } | 获取或设置是否允许其他图表元素与此图表元素重叠。 |
| [IsResizeShapeToFitText](../../aspose.cells.charts/charttextframe/isresizeshapetofittext) { get; set; } | 获取或设置形状是否应自动适应以完全包含其中描述的文本。自动拟合是 当形状内的文本被缩放以包含所有文本时。 |
| virtual [IsTextWrapped](../../aspose.cells.charts/charttextframe/istextwrapped) { get; set; } | 获取或设置一个指示文本是否被换行的值。 |
| [LegendEntries](../../aspose.cells.charts/legend/legendentries) { get; } | 获取指定图表图例中所有 LegendEntry 对象的集合。 不支持设置曲面图的图例条目。 因此，如果图表类型为曲面图表类型，它将返回 null。 |
| [LegendEntriesLabels](../../aspose.cells.charts/legend/legendentrieslabels) { get; } | 调用 Chart.Calculate() 方法后获取图例条目的标签。 |
| virtual [LinkedSource](../../aspose.cells.charts/charttextframe/linkedsource) { get; set; } | 获取并设置对工作表的引用。 |
| [Position](../../aspose.cells.charts/legend/position) { get; set; } | 获取或设置图例位置类型。 |
| [ReadingOrder](../../aspose.cells.charts/charttextframe/readingorder) { get; set; } | 表示文本阅读顺序。 |
| [RotationAngle](../../aspose.cells.charts/charttextframe/rotationangle) { get; set; } | 代表文字旋转角度。 |
| [Shadow](../../aspose.cells.charts/chartframe/shadow) { get; set; } | 如果框架有阴影，则为真。 |
| [ShapeProperties](../../aspose.cells.charts/chartframe/shapeproperties) { get; } | 获取[`ShapeProperties`](../chartframe/shapeproperties)对象。 |
| virtual [Text](../../aspose.cells.charts/charttextframe/text) { get; set; } | 获取或设置框架标题的文本。 |
| [TextHorizontalAlignment](../../aspose.cells.charts/charttextframe/texthorizontalalignment) { get; set; } | 获取和设置文本水平对齐方式。 |
| [TextVerticalAlignment](../../aspose.cells.charts/charttextframe/textverticalalignment) { get; set; } | 获取或设置文本的文本垂直对齐方式。 |
| virtual [Width](../../aspose.cells.charts/chartframe/width) { get; set; } | 获取或设置边框宽度，以图表区域的 1/4000 为单位。 |
| virtual [X](../../aspose.cells.charts/chartframe/x) { get; set; } | 获取或设置图表区域左上角的x坐标，单位为1/4000。 |
| virtual [Y](../../aspose.cells.charts/chartframe/y) { get; set; } | 获取或设置图表区域左上角的y坐标，单位为1/4000。 |

## 方法

| 姓名 | 描述 |
| --- | --- |
| [Characters](../../aspose.cells.charts/charttextframe/characters)(int, int) | 返回一个 Characters 对象，该对象表示文本中的字符范围。 |
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
chart.SetChartDataRange("A1:B4", true);
 //设置图例的宽度和高度
Legend legend = chart.Legend;

//图例默认在图表右侧
 //如果图例在图表的左侧或右侧，设置Legend.X属性将不生效。
 //如果图例在图表的顶部或底部，设置Legend.Y属性将不会生效。
legend.Y = 1500;
legend.Width = 50;
legend.Height = 50; 
 //设置图例的位置
legend.Position = LegendPositionType.Left;

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
		
Dim chartIndex as Integer = sheet.Charts.Add(ChartType.Column, 9, 9, 21, 15)

Dim chart as Chart = sheet.Charts(chartIndex)
chart.SetChartDataRange("A1:B4", True);
 
'设置图例的宽度和高度
Dim legend as Legend = chart.Legend

'图例默认在图表右侧
'如果图例在图表的左侧或右侧，设置Legend.X属性将不生效。
'如果图例在图表的顶部或底部，设置Legend.Y属性将不会生效。             legend.Y = 1500
legend.Width = 50
legend.Height = 50
'设置图例的位置
legend.Position = LegendPositionType.Left
```

### 也可以看看

* class [ChartTextFrame](../charttextframe)
* 命名空间 [Aspose.Cells.Charts](../../aspose.cells.charts)
* 部件 [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
