---
title: ChartDataTable
second_title: Aspose.Cells for .NET API 参考
description: 表示图表数据表
type: docs
weight: 460
url: /zh/net/aspose.cells.charts/chartdatatable/
---
## ChartDataTable class

表示图表数据表。

```csharp
public class ChartDataTable
```

## 特性

| 姓名 | 描述 |
| --- | --- |
| [AutoScaleFont](../../aspose.cells.charts/chartdatatable/autoscalefont) { get; set; } | 如果对象中的文本在对象大小更改时更改字体大小，则为真。 默认值为 True。 |
| [BackgroundMode](../../aspose.cells.charts/chartdatatable/backgroundmode) { get; set; } | 获取和设置背景的显示方式 |
| [Border](../../aspose.cells.charts/chartdatatable/border) { get; } | 返回一个 Border 对象，表示对象的边框 |
| [Font](../../aspose.cells.charts/chartdatatable/font) { get; } | 获取[`Font`](./font)对象，该对象表示指定图表数据表的字体设置。 |
| [HasBorderHorizontal](../../aspose.cells.charts/chartdatatable/hasborderhorizontal) { get; set; } | 如果图表数据表具有水平单元格边框，则为真 |
| [HasBorderOutline](../../aspose.cells.charts/chartdatatable/hasborderoutline) { get; set; } | 如果图表数据表有轮廓边框则为真 |
| [HasBorderVertical](../../aspose.cells.charts/chartdatatable/hasbordervertical) { get; set; } | 如果图表数据表具有垂直单元格边框，则为真 |
| [ShowLegendKey](../../aspose.cells.charts/chartdatatable/showlegendkey) { get; set; } | 如果数据标签图例键可见，则为真。 |

### 例子

```csharp

[C#]

 //实例化一个工作簿对象
Workbook workbook = new Workbook();

//获取第一个worksheet

Worksheet worksheet = workbook.Worksheets[0];

 //向“A1”添加样本值 cell
worksheet.Cells["A1"].PutValue(50);

//向“A2”添加样本值 cell
worksheet.Cells["A2"].PutValue(100);

 //向“A3”添加样本值 cell
worksheet.Cells["A3"].PutValue(150);

 //向“B1”添加样本值 cell
worksheet.Cells["B1"].PutValue(60);

 //将样本值添加到“B2” cell
worksheet.Cells["B2"].PutValue(32);

 //将样本值添加到“B3” cell
worksheet.Cells["B3"].PutValue(50);

 //将图表添加到工作表
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 25, 10);

 //访问新添加的chart

Chart chart = worksheet.Charts[chartIndex];

 //将NSeries（图表数据源）添加到从“A1”单元格到“B3”单元格的图表中
chart.NSeries.Add("A1:B3", true);

chart.ShowDataTable = true;

 //获取图表Table
ChartDataTable chartTable = chart.ChartDataTable;

//设置图表表字体颜色
chartTable.Font.Color = System.Drawing.Color.Red;

 //设置图例键 VisibilityOptions
chartTable.ShowLegendKey = false;

 //保存Excel文件
workbook.Save("book1.xls");

[VB.NET]

'实例化一个Workbook目的
Dim workbook As Workbook = New Workbook()

'Obtaining the reference of the first worksheet
Dim worksheet As Worksheet = workbook.Worksheets(0)

'将样本值添加到至 "A1" cell
worksheet.Cells("A1").PutValue(50)

 "A2" cell
worksheet.Cells("A2").PutValue(100)

'将样本值添加到至 "A3" cell
worksheet.Cells("A3").PutValue(150)

'将样本值添加到至 "B1" cell
worksheet.Cells("B1").PutValue(60)

'将样本值添加到至 "B2" cell
worksheet.Cells("B2").PutValue(32)

'将样本值添加到至 "B3" cell
worksheet.Cells("B3").PutValue(50)

'将图表添加到工作表
Dim chartIndex As Integer = worksheet.Charts.Add(ChartType.Column, 5, 0, 25, 10)

'访问新添加图表的实例
Dim chart As Chart = worksheet.Charts(chartIndex)

'将 NSeries（图表数据源）添加到图表中，范围从“A1”单元格到“B3”
chart.NSeries.Add("A1:B3", True)

chart.ShowDataTable = True

'获取图表表
Dim chartTable As ChartDataTable = chart.ChartDataTable

'设置图表表格字体颜色
chartTable.Font.Color = System.Drawing.Color.Red

'设置图例键 VisibilityOptions
chartTable.ShowLegendKey = False

'保存 Excel 文件
workbook.Save("book1.xls")

```

### 也可以看看

* 命名空间 [Aspose.Cells.Charts](../../aspose.cells.charts)
* 部件 [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
