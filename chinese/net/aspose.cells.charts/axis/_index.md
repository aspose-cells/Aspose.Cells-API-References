---
title: Axis
second_title: Aspose.Cells for .NET API 参考
description: 封装表示图表轴的对象
type: docs
weight: 360
url: /zh/net/aspose.cells.charts/axis/
---
## Axis class

封装表示图表轴的对象。

```csharp
public class Axis
```

## 特性

| 姓名 | 描述 |
| --- | --- |
| [Area](../../aspose.cells.charts/axis/area) { get; } | 获取[`Area`](./area). |
| [AxisBetweenCategories](../../aspose.cells.charts/axis/axisbetweencategories) { get; set; } | 表示值轴是否与类别之间的类别轴相交。 |
| [AxisLabels](../../aspose.cells.charts/axis/axislabels) { get; } | 调用Chart.Calculate()方法后获取坐标轴的标签。 |
| [AxisLine](../../aspose.cells.charts/axis/axisline) { get; } | 获取轴的外观。 |
| [BaseUnitScale](../../aspose.cells.charts/axis/baseunitscale) { get; set; } | 表示类别轴的基本单位比例。 |
| [Bins](../../aspose.cells.charts/axis/bins) { get; } | 表示图表上的 bin（直方图/Pareto）axis |
| [CategoryType](../../aspose.cells.charts/axis/categorytype) { get; set; } | 表示类别轴类型。 |
| [CrossAt](../../aspose.cells.charts/axis/crossat) { get; set; } | 表示值轴上类别轴与其相交的点。 |
| [CrossType](../../aspose.cells.charts/axis/crosstype) { get; set; } | 代表[`CrossType`](./crosstype)在另一个轴相交的指定轴上。 |
| [CustUnit](../../aspose.cells.charts/axis/custunit) { get; set; } | 指定显示单位的自定义值。 |
| [DisplayUnit](../../aspose.cells.charts/axis/displayunit) { get; set; } | 表示指定轴的单位标签。 |
| [DisplayUnitLabel](../../aspose.cells.charts/axis/displayunitlabel) { get; } | 表示指定图表中轴上的单位标签。 单位标签对于绘制大值（例如以百万或十亿为单位）很有用。 |
| [HasMultiLevelLabels](../../aspose.cells.charts/axis/hasmultilevellabels) { get; set; } | 指示标签是否应显示为多级。 |
| [IsAutomaticMajorUnit](../../aspose.cells.charts/axis/isautomaticmajorunit) { get; set; } | 表示是否自动分配轴的主要单位。 |
| [IsAutomaticMaxValue](../../aspose.cells.charts/axis/isautomaticmaxvalue) { get; set; } | 表示是否自动分配最大值。 |
| [IsAutomaticMinorUnit](../../aspose.cells.charts/axis/isautomaticminorunit) { get; set; } | 表示是否自动分配轴的次要单位。 |
| [IsAutomaticMinValue](../../aspose.cells.charts/axis/isautomaticminvalue) { get; set; } | 表示是否自动分配最小值。 |
| [IsAutoTickLabelSpacing](../../aspose.cells.charts/axis/isautoticklabelspacing) { get; set; } | 表示刻度标签的间距是否为自动 |
| [IsDisplayUnitLabelShown](../../aspose.cells.charts/axis/isdisplayunitlabelshown) { get; set; } | 表示显示单位标签是否显示在指定轴上。 |
| [IsLogarithmic](../../aspose.cells.charts/axis/islogarithmic) { get; set; } | 表示数值轴刻度类型是否为对数。 |
| [IsPlotOrderReversed](../../aspose.cells.charts/axis/isplotorderreversed) { get; set; } | 表示 Microsoft Excel 是否从最后一个到第一个绘制数据点。 |
| [IsVisible](../../aspose.cells.charts/axis/isvisible) { get; set; } | 表示轴是否可见。 |
| [LogBase](../../aspose.cells.charts/axis/logbase) { get; set; } | 表示对数底。默认值为 10。仅适用于 Excel2007。 |
| [MajorGridLines](../../aspose.cells.charts/axis/majorgridlines) { get; } | 表示图表轴上的主要网格线。 |
| [MajorTickMark](../../aspose.cells.charts/axis/majortickmark) { get; set; } | 表示指定轴的主要刻度线的类型。 |
| [MajorUnit](../../aspose.cells.charts/axis/majorunit) { get; set; } | 表示轴的主要单位。 |
| [MajorUnitScale](../../aspose.cells.charts/axis/majorunitscale) { get; set; } | 表示类别轴的主要单位比例。 |
| [MaxValue](../../aspose.cells.charts/axis/maxvalue) { get; set; } | 表示数值轴上的最大值。 |
| [MinorGridLines](../../aspose.cells.charts/axis/minorgridlines) { get; } | 表示图表轴上的次要网格线。 |
| [MinorTickMark](../../aspose.cells.charts/axis/minortickmark) { get; set; } | 表示指定轴的次刻度线类型。 |
| [MinorUnit](../../aspose.cells.charts/axis/minorunit) { get; set; } | 表示轴的次要单位。 |
| [MinorUnitScale](../../aspose.cells.charts/axis/minorunitscale) { get; set; } | 表示类别轴的主要单位比例。 |
| [MinValue](../../aspose.cells.charts/axis/minvalue) { get; set; } | 表示数值轴上的最小值。 |
| [TickLabelPosition](../../aspose.cells.charts/axis/ticklabelposition) { get; set; } | 表示指定轴上刻度线标签的位置。 |
| [TickLabels](../../aspose.cells.charts/axis/ticklabels) { get; } | 返回一个[`TickLabels`](./ticklabels)表示指定轴的刻度线标签的对象。 |
| [TickLabelSpacing](../../aspose.cells.charts/axis/ticklabelspacing) { get; set; } | 表示刻度标签之间的类别或系列的数量。仅适用于类别和系列轴。 |
| [TickMarkSpacing](../../aspose.cells.charts/axis/tickmarkspacing) { get; set; } | 返回或设置刻度线之间的类别或系列的数量。仅适用于类别和系列轴。 |
| [Title](../../aspose.cells.charts/axis/title) { get; } | 获取轴的标题。 |

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
//向“B1”单元格添加样本值
worksheet.Cells["B1"].PutValue(4);
//向“B2”单元格添加样本值
worksheet.Cells["B2"].PutValue(20);
//向“B3”单元格添加样本值
worksheet.Cells["B3"].PutValue(50);
//向工作表添加图表
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 25, 5);
//访问新添加图表的实例
Chart chart = worksheet.Charts[chartIndex];
//将NSeries（图表数据源）添加到从“A1”单元格到“B3”单元格的图表中
chart.NSeries.Add("A1:B3", true);
//设置值轴的最大值
chart.ValueAxis.MaxValue = 200;
//设置值轴的最小值
chart.ValueAxis.MinValue = 0;
//设置主要单位
chart.ValueAxis.MajorUnit = 25;
//类别（X）轴在最大值处交叉。
chart.ValueAxis.CrossType = CrossType.Maximum;
//设置刻度标签之间的类别数或系列数。 
chart.CategoryAxis.TickLabelSpacing = 2;

//做你的事

//保存Excel文件
workbook.Save("book1.xlsx");

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
'Adding a sample value to "B1" cell
worksheet.Cells("B1").PutValue(4)
'Adding a sample value to "B2" cell
worksheet.Cells("B2").PutValue(20)
'Adding a sample value to "B3" cell
worksheet.Cells("B3").PutValue(50)
'将图表添加到工作表
Dim chartIndex As Int32 = worksheet.Charts.Add(ChartType.Column, 5, 0, 25, 5)
'访问新添加图表的实例
Dim chart As Chart = worksheet.Charts(chartIndex)
'Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B3"
chart.NSeries.Add("A1:B3", True)
'设置值轴的最大值
chart.ValueAxis.MaxValue = 200
'设置数值轴的最小值
chart.ValueAxis.MinValue = 0
'设置主要单位
chart.ValueAxis.MajorUnit = 25
'Category(X) 轴在最大值处交叉。
chart.ValueAxis.CrossType = CrossType.Maximum
'在刻度线标签之间设置类别或系列的数量。 
chart.CategoryAxis.TickLabelSpacing = 2
'保存 Excel 文件
workbook.Save("book1.xlsx")
```

### 也可以看看

* 命名空间 [Aspose.Cells.Charts](../../aspose.cells.charts)
* 部件 [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
