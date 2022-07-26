---
title: SeriesCollection
second_title: Aspose.Cells for .NET API 参考
description: 封装了一个集合Series./series对象.
type: docs
weight: 830
url: /zh/net/aspose.cells.charts/seriescollection/
---
## SeriesCollection class

封装了一个集合[`Series`](../series)对象.

```csharp
public class SeriesCollection : CollectionBase<Series>
```

## 特性

| 姓名 | 描述 |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase`1/capacity) { get; set; } |  |
| [CategoryData](../../aspose.cells.charts/seriescollection/categorydata) { get; set; } | 获取或设置类别轴值的范围。 可以是单元格范围（例如，“d1:e10”）、 或一系列值（例如，“{2,6,8,10}”）。 |
| [Count](../../aspose.cells/collectionbase`1/count) { get; } |  |
| [IsColorVaried](../../aspose.cells.charts/seriescollection/iscolorvaried) { get; set; } | 表示点的颜色是否变化。 |
| [Item](../../aspose.cells.charts/seriescollection/item) { get; } | 获取[`Series`](../series)指定索引处的元素。 |
| [Item](../../aspose.cells/collectionbase`1/item) { get; set; } |  |
| [SecondCategoryData](../../aspose.cells.charts/seriescollection/secondcategorydata) { get; set; } | 获取或设置第二类轴值的范围。 可以是单元格范围（例如，“d1:e10”）、 或一系列值（例如，“{2,6,8,10}”）。 仅当某些 ASeries 绘制在第二个轴上时才会产生影响。 |

## 方法

| 姓名 | 描述 |
| --- | --- |
| [Add](../../aspose.cells.charts/seriescollection/add#add)(string, bool) | 添加[`SeriesCollection`](../seriescollection)收集到图表。 |
| [Add](../../aspose.cells.charts/seriescollection/add#add_1)(string, bool, bool) | 添加[`SeriesCollection`](../seriescollection)收集到图表。 |
| [AddR1C1](../../aspose.cells.charts/seriescollection/addr1c1)(string, bool) | 添加[`SeriesCollection`](../seriescollection)收集到图表。 |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(Series) |  |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(Series, IComparer&lt;Series&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(int, int, Series, IComparer&lt;Series&gt;) |  |
| [ChangeSeriesOrder](../../aspose.cells.charts/seriescollection/changeseriesorder)(int, int) | 直接改变两个系列的顺序 |
| [Clear](../../aspose.cells.charts/seriescollection/clear#clear)() | 清除集合 (2 methods) |
| [Contains](../../aspose.cells/collectionbase`1/contains)(Series) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(Series[]) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(Series[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(int, Series[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase`1/exists)(Predicate&lt;Series&gt;) |  |
| [Find](../../aspose.cells/collectionbase`1/find)(Predicate&lt;Series&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase`1/findall)(Predicate&lt;Series&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(Predicate&lt;Series&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(int, Predicate&lt;Series&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(int, int, Predicate&lt;Series&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase`1/findlast)(Predicate&lt;Series&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(Predicate&lt;Series&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(int, Predicate&lt;Series&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(int, int, Predicate&lt;Series&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase`1/getenumerator)() |  |
| [GetSeriesByOrder](../../aspose.cells.charts/seriescollection/getseriesbyorder)(int) | 获取[`Series`](../series)按顺序排列元素。 |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(Series) |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(Series, int) |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(Series, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(Series) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(Series, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(Series, int, int) |  |
| [RemoveAt](../../aspose.cells.charts/seriescollection/removeat#removeat)(int) | 删除特定索引处的系列。 (2 methods) |
| [SetSeriesNames](../../aspose.cells.charts/seriescollection/setseriesnames)(int, string, bool) | 设置图表中所有系列的名称。 |

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
//保存Excel文件
workbook.Save("book1.xls");

[Visual Basic]

'实例化工作簿对象
Dim workbook As Workbook = New Workbook()
'向 Excel 对象添加新工作表
Dim sheetIndex As Integer = workbook.Worksheets.Add()
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
Dim chartIndex As Integer = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5)
'访问新添加图表的实例
Dim chart As Chart = worksheet.Charts(chartIndex)
'Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B4"
chart.NSeries.Add("A1:B4", True)
'设置 NSeries 类别数据的数据源
chart.NSeries.CategoryData = "C1:C4"
'保存 Excel 文件
workbook.Save("book1.xls")
```

### 也可以看看

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1)
* class [Series](../series)
* 命名空间 [Aspose.Cells.Charts](../../aspose.cells.charts)
* 部件 [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
