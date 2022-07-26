---
title: DataLabels
second_title: Aspose.Cells for .NET API 参考
description: 封装指定 Series 的所有 DataLabel 对象的集合
type: docs
weight: 580
url: /zh/net/aspose.cells.charts/datalabels/
---
## DataLabels class

封装指定 Series 的所有 DataLabel 对象的集合。

```csharp
public class DataLabels : ChartTextFrame
```

## 特性

| 姓名 | 描述 |
| --- | --- |
| override [Area](../../aspose.cells.charts/datalabels/area) { get; } | 获取[`区域`](./area). |
| virtual [AutoScaleFont](../../aspose.cells.charts/chartframe/autoscalefont) { get; set; } | 如果对象中的文本在对象大小更改时更改字体大小，则为真。默认值是true。 |
| [BackgroundMode](../../aspose.cells.charts/datalabels/backgroundmode) { get; set; } | 获取和设置背景的显示模式 |
| override [Border](../../aspose.cells.charts/datalabels/border) { get; } | 获取[`边界`](../../aspose.cells.drawing/line). |
| [DefaultHeight](../../aspose.cells.charts/chartframe/defaultheight) { get; } | 表示默认位置的高度 |
| [DefaultWidth](../../aspose.cells.charts/chartframe/defaultwidth) { get; } | 表示默认位置的宽度 |
| [DefaultX](../../aspose.cells.charts/chartframe/defaultx) { get; } | 代表默认位置的 x |
| [DefaultY](../../aspose.cells.charts/chartframe/defaulty) { get; } | 代表默认位置的y |
| override [DirectionType](../../aspose.cells.charts/datalabels/directiontype) { get; set; } | 获取和设置文本的方向。 |
| override [Font](../../aspose.cells.charts/datalabels/font) { get; } | 获取DataLabels的字体； |
| virtual [Height](../../aspose.cells.charts/chartframe/height) { get; set; } | 获取或设置边框高度，单位为图表区域的1/4000。 |
| virtual [IsAutomaticSize](../../aspose.cells.charts/chartframe/isautomaticsize) { get; set; } | 指示图表框是否自动调整大小。 |
| override [IsAutoText](../../aspose.cells.charts/datalabels/isautotext) { get; set; } | 表示文本是自动生成的。 |
| [IsDefaultPosBeSet](../../aspose.cells.charts/chartframe/isdefaultposbeset) { get; } | 表示是否设置了默认位置（DefaultX、DefaultY、DefaultWidth 和 DefaultHeight）。 |
| [IsDeleted](../../aspose.cells.charts/charttextframe/isdeleted) { get; set; } | 表示此数据标签是否被删除。 |
| [IsInnerMode](../../aspose.cells.charts/chartframe/isinnermode) { get; set; } | 表示绘图区域大小的大小是否包含刻度线和轴标签。 False 指定大小应确定绘图区域的大小、刻度线和轴标签。 |
| [IsNeverOverlap](../../aspose.cells.charts/datalabels/isneveroverlap) { get; set; } | 指示数据标签显示是否从不重叠。 （对于饼图） |
| [IsResizeShapeToFitText](../../aspose.cells.charts/charttextframe/isresizeshapetofittext) { get; set; } | 获取或设置一个形状是否应该自动适应以完全包含其中描述的文本。当形状内的文本被缩放以包含其中的所有文本时，自动拟合 is 。 |
| override [IsTextWrapped](../../aspose.cells.charts/datalabels/istextwrapped) { get; set; } | 获取或设置一个值，该值指示文本是否被换行。 |
| virtual [LinkedSource](../../aspose.cells.charts/charttextframe/linkedsource) { get; set; } | 获取并设置对工作表的引用。 |
| [Number](../../aspose.cells.charts/datalabels/number) { get; set; } | 获取和设置内置数字格式。 |
| [NumberFormat](../../aspose.cells.charts/datalabels/numberformat) { get; set; } | 表示 DataLabels 对象的格式字符串。 |
| [NumberFormatLinked](../../aspose.cells.charts/datalabels/numberformatlinked) { get; set; } | 如果数字格式链接到单元格 则为真（因此当单元格中的数字格式发生变化时，标签中的数字格式也会发生变化）。 |
| [Position](../../aspose.cells.charts/datalabels/position) { get; set; } | 表示数据标签的位置。 |
| [ReadingOrder](../../aspose.cells.charts/charttextframe/readingorder) { get; set; } | 代表文字阅读顺序。 |
| [RotationAngle](../../aspose.cells.charts/charttextframe/rotationangle) { get; set; } | 代表文字旋转角度。 |
| [SeparatorType](../../aspose.cells.charts/datalabels/separatortype) { get; set; } | 获取或设置用于图表上数据标签的分隔符类型。 |
| [SeparatorValue](../../aspose.cells.charts/datalabels/separatorvalue) { get; set; } | 获取或设置用于图表上数据标签的分隔符值。 |
| [Shadow](../../aspose.cells.charts/chartframe/shadow) { get; set; } | 如果框架有阴影则为真。 |
| [ShapeProperties](../../aspose.cells.charts/chartframe/shapeproperties) { get; } | 获取[`ShapeProperties`](../chartframe/shapeproperties)对象. |
| [ShapeType](../../aspose.cells.charts/datalabels/shapetype) { get; set; } | 获取或设置数据标签的形状类型。 |
| [ShowBubbleSize](../../aspose.cells.charts/datalabels/showbubblesize) { get; set; } | 表示指定图表的数据标签百分比值显示行为。 True 显示百分比值。虚假隐藏。 |
| [ShowCategoryName](../../aspose.cells.charts/datalabels/showcategoryname) { get; set; } | 表示指定图表的数据标签类别名称显示行为。True 为在图表上显示数据标签的类别名称。假隐藏。 |
| [ShowCellRange](../../aspose.cells.charts/datalabels/showcellrange) { get; set; } | 表示是否将单元格区域显示为数据标签。 |
| [ShowLegendKey](../../aspose.cells.charts/datalabels/showlegendkey) { get; set; } | 表示指定图表的数据标签图例键显示行为。 如果数据标签图例键可见则为真。 |
| [ShowPercentage](../../aspose.cells.charts/datalabels/showpercentage) { get; set; } | 表示指定图表的数据标签百分比值显示行为。 True 显示百分比值。虚假隐藏。 |
| [ShowSeriesName](../../aspose.cells.charts/datalabels/showseriesname) { get; set; } | 返回或设置一个布尔值以指示图表上数据标签的系列名称显示行为。 True 以显示系列名称。假隐藏。 |
| [ShowValue](../../aspose.cells.charts/datalabels/showvalue) { get; set; } | 表示指定图表的数据标签值显示行为。 True 显示值。虚假隐藏。 |
| override [Text](../../aspose.cells.charts/datalabels/text) { get; set; } | 获取或设置数据标签的文本。 |
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

//设置图表中的DataLabels
DataLabels datalabels;
for (int i = 0; i  <chart.NSeries.Count; i++)
{
    datalabels = chart.NSeries[i].DataLabels;
    //设置DataLabels的位置
    datalabels.Position = LabelPositionType.InsideBase;
    //在DataLabels中显示类别名称
    datalabels.ShowCategoryName = true;
    //显示DataLabels中的值
    datalabels.ShowValue = true;
    //不显示DataLabels中的百分比
    datalabels.ShowPercentage = false;
    //不显示图例键。
    datalabels.ShowLegendKey = false;
}

[Visual Basic]

'在图表中设置 DataLabels
Dim datalabels As DataLabels
Dim i As Integer
For i = 0 To chart.NSeries.Count - 1 Step 1
    datalabels = chart.NSeries(i).DataLabels
    '设置 DataLabels 的位置
    datalabels.Position = LabelPositionType.InsideBase
    '在 DataLabels 中显示类别名称
    datalabels.ShowCategoryName= True
    '在 DataLabels 中显示值
    datalabels.ShowValue = True
    '不在 DataLabels 中显示百分比
    datalabels.ShowPercentage = False
    '不显示图例键。
    datalabels.ShowLegendKey = False
Next
```

### 也可以看看

* class [ChartTextFrame](../charttextframe)
* 命名空间 [Aspose.Cells.Charts](../../aspose.cells.charts)
* 部件 [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
