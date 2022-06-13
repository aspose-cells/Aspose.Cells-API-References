---
title: TimelineCollection
second_title: Aspose.Cells for .NET API 参考
description: 指定指定工作表上所有时间轴对象的集合
type: docs
weight: 6080
url: /zh/net/aspose.cells.timelines/timelinecollection/
---
## TimelineCollection class

指定指定工作表上所有时间轴对象的集合。

```csharp
public class TimelineCollection : CollectionBase<Timeline>
```

## 特性

| 姓名 | 描述 |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase`1/capacity) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase`1/count) { get; } |  |
| [Item](../../aspose.cells.timelines/timelinecollection/item) { get; } | 按索引获取时间轴。 (2 indexers) |
| [Item](../../aspose.cells/collectionbase`1/item) { get; set; } |  |

## 方法

| 姓名 | 描述 |
| --- | --- |
| [Add](../../aspose.cells.timelines/timelinecollection/add#add_4)(PivotTable, string, int) | 使用数据透视表作为数据源添加新时间线 |
| [Add](../../aspose.cells.timelines/timelinecollection/add#add_3)(PivotTable, string, PivotField) | 使用数据透视表作为数据源添加新时间线 |
| [Add](../../aspose.cells.timelines/timelinecollection/add#add_5)(PivotTable, string, string) | 使用数据透视表作为数据源添加新时间线 |
| [Add](../../aspose.cells.timelines/timelinecollection/add#add_1)(PivotTable, int, int, int) | 使用数据透视表作为数据源添加新时间线 |
| [Add](../../aspose.cells.timelines/timelinecollection/add#add)(PivotTable, int, int, PivotField) | 使用数据透视表作为数据源添加新时间线 |
| [Add](../../aspose.cells.timelines/timelinecollection/add#add_2)(PivotTable, int, int, string) | 使用数据透视表作为数据源添加新时间线 |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(Timeline) |  |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(Timeline, IComparer&lt;Timeline&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(int, int, Timeline, IComparer&lt;Timeline&gt;) |  |
| [Clear](../../aspose.cells/collectionbase`1/clear)() |  |
| [Contains](../../aspose.cells/collectionbase`1/contains)(Timeline) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(Timeline[]) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(Timeline[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(int, Timeline[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase`1/exists)(Predicate&lt;Timeline&gt;) |  |
| [Find](../../aspose.cells/collectionbase`1/find)(Predicate&lt;Timeline&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase`1/findall)(Predicate&lt;Timeline&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(Predicate&lt;Timeline&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(int, Predicate&lt;Timeline&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(int, int, Predicate&lt;Timeline&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase`1/findlast)(Predicate&lt;Timeline&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(Predicate&lt;Timeline&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(int, Predicate&lt;Timeline&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(int, int, Predicate&lt;Timeline&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase`1/getenumerator)() |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(Timeline) |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(Timeline, int) |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(Timeline, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(Timeline) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(Timeline, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(Timeline, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase`1/removeat)(int) |  |

### 例子

```csharp

[C#]
Workbook book = new Workbook();
Worksheet sheet = book.Worksheets[0];
Cells cells = sheet.Cells;
cells[0, 0].Value = "fruit";
cells[1, 0].Value = "grape";
cells[2, 0].Value = "blueberry";
cells[3, 0].Value = "kiwi";
cells[4, 0].Value = "cherry";

 //创建日期样式
Style dateStyle = new CellsFactory().CreateStyle();
dateStyle.Custom = "m/d/yyyy";
cells[0, 1].Value = "date";
cells[1, 1].Value = new DateTime(2021, 2, 5);
cells[2, 1].Value = new DateTime(2022, 3, 8);
cells[3, 1].Value = new DateTime(2023, 4, 10);
cells[4, 1].Value = new DateTime(2024, 5, 16);
 //设置日期样式
cells[1, 1].SetStyle(dateStyle);
cells[2, 1].SetStyle(dateStyle);
cells[3, 1].SetStyle(dateStyle);
cells[4, 1].SetStyle(dateStyle);

cells[0, 2].Value = "amount";
cells[1, 2].Value = 50;
cells[2, 2].Value = 60;
cells[3, 2].Value = 70;
cells[4, 2].Value = 80;

PivotTableCollection pivots = sheet.PivotTables;
 //添加一个数据透视表
int pivotIndex = pivots.Add("=Sheet1!A1:C5", "A12", "TestPivotTable");
PivotTable pivot = pivots[pivotIndex];
pivot.AddFieldToArea(PivotFieldType.Row, "fruit");
pivot.AddFieldToArea(PivotFieldType.Column, "date");
pivot.AddFieldToArea(PivotFieldType.Data, "amount");
pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;

 //刷新数据透视表data
pivot.RefreshData();
pivot.CalculateData();

 //做你的事
book.Save("out.xlsx");

```

### 也可以看看

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1)
* class [Timeline](../timeline)
* 命名空间 [Aspose.Cells.Timelines](../../aspose.cells.timelines)
* 部件 [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
