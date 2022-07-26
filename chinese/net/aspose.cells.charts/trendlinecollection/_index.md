---
title: TrendlineCollection
second_title: Aspose.Cells for .NET API 参考
description: 代表所有的集合Trendline./trendline指定数据系列的对象
type: docs
weight: 990
url: /zh/net/aspose.cells.charts/trendlinecollection/
---
## TrendlineCollection class

代表所有的集合[`Trendline`](../trendline)指定数据系列的对象。

```csharp
public class TrendlineCollection : CollectionBase<Trendline>
```

## 特性

| 姓名 | 描述 |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase`1/capacity) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase`1/count) { get; } |  |
| [Item](../../aspose.cells.charts/trendlinecollection/item) { get; } | 得到一个对象的索引。 |
| [Item](../../aspose.cells/collectionbase`1/item) { get; set; } |  |

## 方法

| 姓名 | 描述 |
| --- | --- |
| [Add](../../aspose.cells.charts/trendlinecollection/add#add)(TrendlineType) | 添加一个具有指定类型的此集合的对象。 |
| [Add](../../aspose.cells.charts/trendlinecollection/add#add_1)(TrendlineType, string) | 添加一个具有指定类型和名称的此集合的对象。 |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(Trendline) |  |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(Trendline, IComparer&lt;Trendline&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(int, int, Trendline, IComparer&lt;Trendline&gt;) |  |
| [Clear](../../aspose.cells/collectionbase`1/clear)() |  |
| [Contains](../../aspose.cells/collectionbase`1/contains)(Trendline) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(Trendline[]) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(Trendline[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(int, Trendline[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase`1/exists)(Predicate&lt;Trendline&gt;) |  |
| [Find](../../aspose.cells/collectionbase`1/find)(Predicate&lt;Trendline&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase`1/findall)(Predicate&lt;Trendline&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(Predicate&lt;Trendline&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(int, Predicate&lt;Trendline&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(int, int, Predicate&lt;Trendline&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase`1/findlast)(Predicate&lt;Trendline&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(Predicate&lt;Trendline&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(int, Predicate&lt;Trendline&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(int, int, Predicate&lt;Trendline&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase`1/getenumerator)() |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(Trendline) |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(Trendline, int) |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(Trendline, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(Trendline) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(Trendline, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(Trendline, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase`1/removeat)(int) |  |

### 例子

```csharp
[C#]

//实例化一个工作簿对象
Workbook workbook = new Workbook();
//向Excel对象添加一个新的工作表
int sheetIndex = workbook.Worksheets.Add();
//通过传入工作表的索引来获取新添加的工作表的引用
Worksheet worksheet = workbook.Worksheets[sheetIndex];
worksheet.Cells["A1"].PutValue(50);
worksheet.Cells["A2"].PutValue(100);
worksheet.Cells["A3"].PutValue(150);
worksheet.Cells["A4"].PutValue(200);
worksheet.Cells["B1"].PutValue(60);
worksheet.Cells["B2"].PutValue(32);
worksheet.Cells["B3"].PutValue(50);
worksheet.Cells["B4"].PutValue(40);

//向工作表添加图表
int chartIndex = workbook.Worksheets[0].Charts.Add(ChartType.Column, 3, 3, 15, 10);
Chart chart = workbook.Worksheets[0].Charts[chartIndex];
chart.NSeries.Add("A1:a3", true);
chart.NSeries[0].TrendLines.Add(TrendlineType.Linear, "MyTrendLine");
Trendline line = chart.NSeries[0].TrendLines[0];
line.DisplayEquation = true;
line.DisplayRSquared = true;
line.Color = Color.Red;

[Visual Basic]

'实例化工作簿对象
Dim workbook As Workbook = New Workbook()
'向 Excel 对象添加新工作表
Dim sheetIndex As Int32 = workbook.Worksheets.Add()
'通过传入工作表的索引来获取新添加的工作表的引用
Dim worksheet As Worksheet = workbook.Worksheets(sheetIndex)
worksheet.Cells("A1").PutValue(50)
worksheet.Cells("A2").PutValue(100)
worksheet.Cells("A3").PutValue(150)
worksheet.Cells("A4").PutValue(200)
worksheet.Cells("B1").PutValue(60)
worksheet.Cells("B2").PutValue(32)
worksheet.Cells("B3").PutValue(50)
worksheet.Cells("B4").PutValue(40)

'将图表添加到工作表
Dim chartIndex As Integer =  workbook.Worksheets(0).Charts.Add(ChartType.Column,3,3,15,10) 
Dim chart As Chart =  workbook.Worksheets(0).Charts(chartIndex) 
chart.NSeries.Add("A1:a3", True)
chart.NSeries(0).TrendLines.Add(TrendlineType.Linear, "MyTrendLine")
Dim line As Trendline =  chart.NSeries(0).TrendLines(0) 
line.DisplayEquation = True
line.DisplayRSquared = True
line.Color = Color.Red
```

### 也可以看看

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1)
* class [Trendline](../trendline)
* 命名空间 [Aspose.Cells.Charts](../../aspose.cells.charts)
* 部件 [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
