---
title: Trendline
second_title: Aspose.Cells for .NET API 参考
description: 表示图表中的趋势线
type: docs
weight: 980
url: /zh/net/aspose.cells.charts/trendline/
---
## Trendline class

表示图表中的趋势线。

```csharp
public class Trendline : Line
```

## 特性

| 姓名 | 描述 |
| --- | --- |
| [Backward](../../aspose.cells.charts/trendline/backward) { get; set; } | 返回或设置趋势线向后延伸的周期数（或散点图上的单位）。 周期数必须大于等于0 |
| [BeginArrowLength](../../aspose.cells.drawing/line/beginarrowlength) { get; set; } | 指定行首的箭头长度。 |
| [BeginArrowWidth](../../aspose.cells.drawing/line/beginarrowwidth) { get; set; } | 指定行首箭头的宽度。 |
| [BeginType](../../aspose.cells.drawing/line/begintype) { get; set; } | 指定行首的箭头。 |
| [CapType](../../aspose.cells.drawing/line/captype) { get; set; } | 指定结尾大写。 |
| [Color](../../aspose.cells.drawing/line/color) { get; set; } | 代表Color行的. |
| [CompoundType](../../aspose.cells.drawing/line/compoundtype) { get; set; } | 指定复合线型 |
| [DashType](../../aspose.cells.drawing/line/dashtype) { get; set; } | 指定虚线类型 |
| [DataLabels](../../aspose.cells.charts/trendline/datalabels) { get; } | 表示指定系列的 DataLabels 对象。 |
| [DisplayEquation](../../aspose.cells.charts/trendline/displayequation) { get; set; } | 表示趋势线的方程是否显示在图表上（在与 R 平方值相同的数据标签中）。将此属性设置为 True 会自动打开数据标签。 |
| [DisplayRSquared](../../aspose.cells.charts/trendline/displayrsquared) { get; set; } | 表示趋势线的 R 平方值是否显示在图表上（在与方程相同的数据标签中）。将此属性设置为 True 会自动打开数据标签。 |
| [EndArrowLength](../../aspose.cells.drawing/line/endarrowlength) { get; set; } | 指定行尾的箭头长度。 |
| [EndArrowWidth](../../aspose.cells.drawing/line/endarrowwidth) { get; set; } | 指定行尾的箭头宽度。 |
| [EndType](../../aspose.cells.drawing/line/endtype) { get; set; } | 指定行尾的箭头。 |
| [FormattingType](../../aspose.cells.drawing/line/formattingtype) { get; set; } | 获取或设置格式类型。 |
| [Forward](../../aspose.cells.charts/trendline/forward) { get; set; } | 返回或设置趋势线向前延伸的周期数（或散点图上的单位）。 周期数必须大于或等于零。 |
| [GradientFill](../../aspose.cells.drawing/line/gradientfill) { get; } | 表示渐变填充。 |
| [Intercept](../../aspose.cells.charts/trendline/intercept) { get; set; } | 返回或设置趋势线与数值轴相交的点。 |
| [IsAuto](../../aspose.cells.drawing/line/isauto) { get; set; } | 指示此线型是否自动分配。 |
| [IsAutomaticColor](../../aspose.cells.drawing/line/isautomaticcolor) { get; } | 表示线的颜色是否自动分配。 |
| [IsNameAuto](../../aspose.cells.charts/trendline/isnameauto) { get; set; } | 如果 Microsoft Excel 自动确定趋势线的名称，则返回。 |
| [IsVisible](../../aspose.cells.drawing/line/isvisible) { get; set; } | 表示线是否可见。 |
| [JoinType](../../aspose.cells.drawing/line/jointype) { get; set; } | 指定连接大写字母。 |
| [LegendEntry](../../aspose.cells.charts/trendline/legendentry) { get; } | 根据这条趋势线获取图例条目 |
| [Name](../../aspose.cells.charts/trendline/name) { get; set; } | 返回趋势线的名称。 |
| [Order](../../aspose.cells.charts/trendline/order) { get; set; } | 当趋势线类型为多项式时，返回或设置趋势线顺序（大于 1 的整数）。 顺序必须在 2 到 6 之间。 |
| [Period](../../aspose.cells.charts/trendline/period) { get; set; } | 返回或设置移动平均趋势线的周期。 |
| [Style](../../aspose.cells.drawing/line/style) { get; set; } | 代表线条的样式。 |
| [ThemeColor](../../aspose.cells.drawing/line/themecolor) { get; set; } | 获取和设置主题颜色。 |
| [Transparency](../../aspose.cells.drawing/line/transparency) { get; set; } | 将线条的透明度返回或设置为从 0.0（不透明）到 1.0（透明）的值。 |
| [Type](../../aspose.cells.charts/trendline/type) { get; } | 返回趋势线类型。 |
| [Weight](../../aspose.cells.drawing/line/weight) { get; set; } | 获取或设置[`WeightType`](../../aspose.cells.drawing/weighttype)行的. |
| [WeightPt](../../aspose.cells.drawing/line/weightpt) { get; set; } | 获取或设置线的权重，以点为单位。 |
| [WeightPx](../../aspose.cells.drawing/line/weightpx) { get; set; } | 获取或设置线条的权重，以像素为单位。 |

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
//添加线性趋势线
int index = chart.NSeries[0].TrendLines.Add(TrendlineType.Linear);
Trendline trendline = chart.NSeries[0].TrendLines[index];
//设置趋势线的自定义名称。
trendline.Name = "Linear";
//在图表上显示方程
trendline.DisplayEquation = true;
//在图表上显示R平方值
trendline.DisplayRSquared = true;
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
'添加线性趋势线
Dim index As Int32 = chart.NSeries(0).TrendLines.Add(TrendlineType.Linear)
Dim trendline As Trendline = chart.NSeries(0).TrendLines(index)
'设置趋势线的自定义名称。
trendline.Name = "Linear"
'在图表上显示方程
trendline.DisplayEquation = True
'在图表上显示 R 平方值
trendline.DisplayRSquared = True
'保存 Excel 文件
workbook.Save("book1.xls")
```

### 也可以看看

* class [Line](../../aspose.cells.drawing/line)
* 命名空间 [Aspose.Cells.Charts](../../aspose.cells.charts)
* 部件 [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
