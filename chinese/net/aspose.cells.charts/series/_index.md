---
title: Series
second_title: Aspose.Cells for .NET API 参考
description: 封装表示图表中单个数据系列的对象
type: docs
weight: 820
url: /zh/net/aspose.cells.charts/series/
---
## Series class

封装表示图表中单个数据系列的对象。

```csharp
public class Series
```

## 特性

| 姓名 | 描述 |
| --- | --- |
| [Area](../../aspose.cells.charts/series/area) { get; } | 表示Series对象的背景区域。 |
| [Bar3DShapeType](../../aspose.cells.charts/series/bar3dshapetype) { get; set; } | 获取或设置用于 3-D 条形图或柱形图的 3D 形状类型。 |
| [Border](../../aspose.cells.charts/series/border) { get; } | 表示Series对象的边框。 |
| [BubbleScale](../../aspose.cells.charts/series/bubblescale) { get; set; } | 获取或设置指定图表组中气泡的比例因子。 可以是从 0（零）到 300 的整数值， 对应于默认大小的百分比。 仅适用于气泡图。 |
| [BubbleSizes](../../aspose.cells.charts/series/bubblesizes) { get; set; } | 获取或设置图表系列的气泡大小值。 |
| [CountOfDataValues](../../aspose.cells.charts/series/countofdatavalues) { get; } | 获取数据值的个数。 |
| [DataLabels](../../aspose.cells.charts/series/datalabels) { get; } | 表示指定 ASeries 的 DataLabels 对象。 |
| [DisplayName](../../aspose.cells.charts/series/displayname) { get; } | 获取显示在图表图形上的系列名称。 |
| [DoughnutHoleSize](../../aspose.cells.charts/series/doughnutholesize) { get; set; } | 返回或设置圆环图组中孔的大小。 孔大小以图表大小的百分比表示，介于 10% 和 90% 之间。 |
| [DownBars](../../aspose.cells.charts/series/downbars) { get; } | 返回一个[`DropBars`](../dropbars)对象，该对象表示折线图上的向下柱。 仅适用于折线图。 |
| [DropLines](../../aspose.cells.charts/series/droplines) { get; } | 返回一个[`Line`](../../aspose.cells.drawing/line)对象，该对象表示折线图或面积图上的系列的下降线. 仅适用于折线图或面积图。 |
| [Explosion](../../aspose.cells.charts/series/explosion) { get; set; } | 一个开放的饼图切片到饼图中心的距离表示为饼图直径的百分比。 |
| [FirstSliceAngle](../../aspose.cells.charts/series/firstsliceangle) { get; set; } | 获取或设置第一个饼图或圆环图切片的角度，以度为单位（从垂直顺时针方向）。 仅适用于饼图、3-D 饼图和圆环图，0 到 360。 |
| [GapWidth](../../aspose.cells.charts/series/gapwidth) { get; set; } | 返回或设置条形或列簇之间的间距，以条形或列宽的百分比表示。 该属性的值必须介于 0 和 500 之间。 |
| [Has3DEffect](../../aspose.cells.charts/series/has3deffect) { get; set; } | 如果系列具有三维外观，则为真。 仅适用于气泡图。 |
| [HasDropLines](../../aspose.cells.charts/series/hasdroplines) { get; set; } | 如果图表有下降线，则为真。 仅适用于折线图或面积图。 |
| [HasHiLoLines](../../aspose.cells.charts/series/hashilolines) { get; set; } | 如果折线图有高低线，则为真。 仅适用于折线图。 |
| [HasLeaderLines](../../aspose.cells.charts/series/hasleaderlines) { get; set; } | 如果系列有引导线，则为真。 |
| [HasRadarAxisLabels](../../aspose.cells.charts/series/hasradaraxislabels) { get; set; } | 如果雷达图有类别轴标签，则为真。仅适用于雷达图。 |
| [HasSeriesLines](../../aspose.cells.charts/series/hasserieslines) { get; set; } | 如果堆积柱形图或条形图有系列线或 如果饼图或饼图之间有连接线，则为真两个部分。 仅适用于堆积柱形图、条形图、饼图或饼图。 |
| [HasUpDownBars](../../aspose.cells.charts/series/hasupdownbars) { get; set; } | 如果折线图有上下柱，则为真。 仅适用于折线图。 |
| [HiLoLines](../../aspose.cells.charts/series/hilolines) { get; } | 返回一个 HiLoLines 对象，该对象表示折线图上系列的高低线。 仅适用于折线图。 |
| [IsAutoSplit](../../aspose.cells.charts/series/isautosplit) { get; } | 表示阈值是否为自动。 |
| [IsColorVaried](../../aspose.cells.charts/series/iscolorvaried) { get; set; } | 表示点的颜色是否变化。 图表必须只包含一个系列。 |
| [IsVerticalValues](../../aspose.cells.charts/series/isverticalvalues) { get; } | 表示数据源是否垂直。 |
| [LayoutProperties](../../aspose.cells.charts/series/layoutproperties) { get; } | 表示布局的属性。 |
| [LeaderLines](../../aspose.cells.charts/series/leaderlines) { get; } | 表示图表上的引导线。引导线将数据标签连接到数据点。 这个对象不是一个集合；没有代表单个引导线的对象。 |
| [LegendEntry](../../aspose.cells.charts/series/legendentry) { get; } | 根据本系列获取图例条目。 |
| [Marker](../../aspose.cells.charts/series/marker) { get; } | 获取[`标记`](./marker) 。 |
| [Name](../../aspose.cells.charts/series/name) { get; set; } | 获取或设置数据系列的名称。 |
| [Overlap](../../aspose.cells.charts/series/overlap) { get; set; } | 指定条和列的定位方式。 可以是介于 – 100 和 100 之间的值。 仅适用于二维条形图和二维柱形图。 |
| [PlotOnSecondAxis](../../aspose.cells.charts/series/plotonsecondaxis) { get; set; } | 指示此系列是否绘制在第二个值轴上。 |
| [Points](../../aspose.cells.charts/series/points) { get; } | 获取图表中一系列点的集合。 |
| [SecondPlotSize](../../aspose.cells.charts/series/secondplotsize) { get; set; } | 返回或设置饼图或饼图条形图的次要部分的大小， 主饼的大小。 可以是 5 到 200 之间的值。 |
| [SeriesLines](../../aspose.cells.charts/series/serieslines) { get; } | 返回一个 SeriesLines 对象，该对象表示堆积条形图或堆积柱形图的系列线。 仅适用于堆积条形图和堆积柱形图。 |
| [Shadow](../../aspose.cells.charts/series/shadow) { get; set; } | 如果系列有阴影，则为真。 |
| [ShapeProperties](../../aspose.cells.charts/series/shapeproperties) { get; } | 获取对象，该对象包含系列的视觉形状属性。 |
| [ShowNegativeBubbles](../../aspose.cells.charts/series/shownegativebubbles) { get; set; } | 如果图表组显示负气泡，则为真。仅对气泡图有效。 |
| [SizeRepresents](../../aspose.cells.charts/series/sizerepresents) { get; set; } | 获取或设置气泡图上的气泡大小。 |
| [Smooth](../../aspose.cells.charts/series/smooth) { get; set; } | 表示曲线平滑。 如果为折线图或散点图打开曲线平滑，则为真。 仅适用于由折线图连接的折线和散点图。 |
| [SplitType](../../aspose.cells.charts/series/splittype) { get; set; } | 返回或设置一个值，该值如何确定哪些数据点在第二个饼图或第二个饼图或饼图上的条形图或 饼图中图表。 |
| [SplitValue](../../aspose.cells.charts/series/splitvalue) { get; set; } | 返回或设置一个值，该值应用于确定 上的第二个饼图或条形图中的数据点饼图集。 |
| [TrendLines](../../aspose.cells.charts/series/trendlines) { get; } | 返回一个对象，该对象表示该系列的所有趋势线的集合。 |
| [Type](../../aspose.cells.charts/series/type) { get; set; } | 获取或设置数据系列的类型。 |
| [UpBars](../../aspose.cells.charts/series/upbars) { get; } | 返回一个 DropBars 对象，该对象表示折线图上的向上柱。 仅适用于折线图。 |
| [Values](../../aspose.cells.charts/series/values) { get; set; } | 表示图表系列的数据。 |
| [ValuesFormatCode](../../aspose.cells.charts/series/valuesformatcode) { get; set; } | 代表Values的NumberList的格式码。 |
| [XErrorBar](../../aspose.cells.charts/series/xerrorbar) { get; } | 表示系列的 X 方向误差条。 |
| [XValues](../../aspose.cells.charts/series/xvalues) { get; set; } | 表示图表系列的 x 值。 |
| [YErrorBar](../../aspose.cells.charts/series/yerrorbar) { get; } | 表示序列的 Y 方向误差条。 |

## 方法

| 姓名 | 描述 |
| --- | --- |
| [Move](../../aspose.cells.charts/series/move)(int) | 向上或向下移动系列。 |

### 例子

```csharp

[C#]

 //实例化一个工作簿对象
Workbook workbook = new Workbook();
 //向Excel对象添加新工作表
int sheetIndex = workbook.Worksheets.Add();
 //通过传入其sheet index
eet的引用
Worksheet worksheet = workbook.Worksheets[sheetIndex];
 //向“A1”添加样本值 cell
worksheet.Cells["A1"].PutValue(50);
//向“A2”添加样本值 cell
worksheet.Cells["A2"].PutValue(100);
 //向“A3”添加样本值 cell
worksheet.Cells["A3"].PutValue(150);
 //向“A4”添加样本值 cell
worksheet.Cells["A4"].PutValue(200);
 //向“B1”添加样本值 cell
worksheet.Cells["B1"].PutValue(60);
 //将样本值添加到“B2” cell
worksheet.Cells["B2"].PutValue(32);
 //将样本值添加到“B3” cell
worksheet.Cells["B3"].PutValue(50);
 //将样本值添加到“B4” cell
worksheet.Cells["B4"].PutValue(40);
 //将样本值添加到“C1”单元格作为类别 data
worksheet.Cells["C1"].PutValue("Q1");
 //将样本值添加到“C2”单元格作为类别 data
worksheet.Cells["C2"].PutValue("Q2");
 //将样本值添加到“C3”单元格作为类别 data
worksheet.Cells["C3"].PutValue("Y1");
 //将样本值添加到“C4”单元格作为类别 data
worksheet.Cells["C4"].PutValue("Y2");
 //将图表添加到工作表
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
 //访问新添加的chart

Chart chart = worksheet.Charts[chartIndex];
//将NSeries（图表数据源）添加到从“A1”单元格到“B4”单元格的图表中
int seriesIndex = chart.NSeries.Add("A1:B4", true);
 //设置NSeries

chart.NSeries.CategoryData = "C1:C4";
Series series = chart.NSeries[seriesIndex];
 //设置series.

series.Values = "=B1:B4";
//更改系列的图表类型
series.Type = ChartType.Line;
 //设置标记属性.
series.Marker.MarkerStyle = ChartMarkerType.Circle;
series.Marker.ForegroundColorSetType = FormattingType.Automatic;
series.Marker.ForegroundColor = System.Drawing.Color.Black;
series.Marker.BackgroundColorSetType = FormattingType.Automatic;

 //做你的事

 //保存Excel文件
workbook.Save("book1.xls");

[Visual Basic]

'实例化一个工作簿对象
Dim workbook As Workbook = New Workbook()
'向 Excel 对象添加新工作表
Dim sheetIndex As Int32 = workbook.Worksheets.Add()
'通过传递其工作表索引来获取新添加工作表的引用
Dim worksheet As Worksheet = workbook.Worksheets(sheetIndex)
'将样本值添加到至 "A1" cell
worksheet.Cells("A1").PutValue(50)
'将样本值添加到至 "A2" cell
worksheet.Cells("A2").PutValue(100)
'将样本值添加到至 "A3" cell
worksheet.Cells("A3").PutValue(150)
'将样本值添加到至 "A4" cell
worksheet.Cells("A4").PutValue(200)
'将样本值添加到至 "B1" cell
worksheet.Cells("B1").PutValue(60)
'将样本值添加到至 "B2" cell
worksheet.Cells("B2").PutValue(32)
'将样本值添加到至 "B3" cell
worksheet.Cells("B3").PutValue(50)
'将样本值添加到至 "B4" cell
worksheet.Cells("B4").PutValue(40)
'将样本值添加到至 "C1" cell as category data
worksheet.Cells("C1").PutValue("Q1")
'将样本值添加到至 "C2" cell as category data
worksheet.Cells("C2").PutValue("Q2")
'将样本值添加到至 "C3" cell as category data
worksheet.Cells("C3").PutValue("Y1")
'将样本值添加到至 "C4" cell as category data
worksheet.Cells("C4").PutValue("Y2")
'将图表添加到工作表
Dim chartIndex As Int32 = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5)
'访问新添加图表的实例
Dim chart As Chart = worksheet.Charts(chartIndex)
'将 NSeries（图表数据源）添加到图表中，范围从“A1”单元格到“B4”
Dim seriesIndex As Int32 = chart.NSeries.Add("A1:B4", True)
'为 NSeries 的类别数据设置数据源
chart.NSeries.CategoryData = "C1:C4"
Dim series As Series = chart.NSeries(seriesIndex)
'设置系列的值。
series.Values = "=B1:B4"
'更改系列的图表类型。
series.Type = ChartType.Line
'设置标记属性。
series.Marker.MarkerStyle = ChartMarkerType.Circle
series.Marker.ForegroundColorSetType = FormattingType.Automatic
series.Marker.ForegroundColor = System.Drawing.Color.Black
series.Marker.BackgroundColorSetType = FormattingType.Automatic
'保存 Excel 文件
workbook.Save("book1.xls")
```

### 也可以看看

* 命名空间 [Aspose.Cells.Charts](../../aspose.cells.charts)
* 部件 [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
