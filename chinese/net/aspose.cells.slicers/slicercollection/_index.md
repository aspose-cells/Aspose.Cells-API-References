---
title: SlicerCollection
second_title: Aspose.Cells for .NET API 参考
description: 指定指定工作表上所有 Slicer 对象的集合
type: docs
weight: 5690
url: /zh/net/aspose.cells.slicers/slicercollection/
---
## SlicerCollection class

指定指定工作表上所有 Slicer 对象的集合。

```csharp
public class SlicerCollection : CollectionBase<Slicer>
```

## 特性

| 姓名 | 描述 |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase`1/capacity) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase`1/count) { get; } |  |
| [Item](../../aspose.cells.slicers/slicercollection/item) { get; } | 通过索引获取切片器。 (2 indexers) |
| [Item](../../aspose.cells/collectionbase`1/item) { get; set; } |  |

## 方法

| 姓名 | 描述 |
| --- | --- |
| [Add](../../aspose.cells.slicers/slicercollection/add#add_8)(ListObject, int, string) | 使用 ListObjet 作为数据源添加新切片器 |
| [Add](../../aspose.cells.slicers/slicercollection/add#add_7)(ListObject, ListColumn, string) | 使用 ListObjet 作为数据源添加新切片器 |
| [Add](../../aspose.cells.slicers/slicercollection/add#add_4)(PivotTable, string, int) | 添加一个使用数据透视表作为数据源的新切片器 |
| [Add](../../aspose.cells.slicers/slicercollection/add#add_3)(PivotTable, string, PivotField) | 添加一个使用数据透视表作为数据源的新切片器 |
| [Add](../../aspose.cells.slicers/slicercollection/add#add_5)(PivotTable, string, string) | 添加一个使用数据透视表作为数据源的新切片器 |
| [Add](../../aspose.cells.slicers/slicercollection/add#add_6)(ListObject, ListColumn, int, int) | 使用 ListObjet 作为数据源添加新切片器 |
| [Add](../../aspose.cells.slicers/slicercollection/add#add_1)(PivotTable, int, int, int) | 添加一个使用数据透视表作为数据源的新切片器 |
| [Add](../../aspose.cells.slicers/slicercollection/add#add)(PivotTable, int, int, PivotField) | 添加一个使用数据透视表作为数据源的新切片器 |
| [Add](../../aspose.cells.slicers/slicercollection/add#add_2)(PivotTable, int, int, string) | 添加一个使用数据透视表作为数据源的新切片器 |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(Slicer) |  |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(Slicer, IComparer&lt;Slicer&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(int, int, Slicer, IComparer&lt;Slicer&gt;) |  |
| [Clear](../../aspose.cells/collectionbase`1/clear)() |  |
| [Contains](../../aspose.cells/collectionbase`1/contains)(Slicer) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(Slicer[]) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(Slicer[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(int, Slicer[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase`1/exists)(Predicate&lt;Slicer&gt;) |  |
| [Find](../../aspose.cells/collectionbase`1/find)(Predicate&lt;Slicer&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase`1/findall)(Predicate&lt;Slicer&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(Predicate&lt;Slicer&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(int, Predicate&lt;Slicer&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(int, int, Predicate&lt;Slicer&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase`1/findlast)(Predicate&lt;Slicer&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(Predicate&lt;Slicer&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(int, Predicate&lt;Slicer&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(int, int, Predicate&lt;Slicer&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase`1/getenumerator)() |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(Slicer) |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(Slicer, int) |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(Slicer, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(Slicer) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(Slicer, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(Slicer, int, int) |  |
| [Remove](../../aspose.cells.slicers/slicercollection/remove)(Slicer) | 移除指定的 Slicer |
| [RemoveAt](../../aspose.cells.slicers/slicercollection/removeat#removeat)(int) | 删除指定索引处的 Slicer (2 methods) |

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
cells[5, 0].Value = "grape";
cells[6, 0].Value = "blueberry";
cells[7, 0].Value = "kiwi";
cells[8, 0].Value = "cherry";

cells[0, 1].Value = "year";
cells[1, 1].Value = 2020;
cells[2, 1].Value = 2020;
cells[3, 1].Value = 2020;
cells[4, 1].Value = 2020;
cells[5, 1].Value = 2021;
cells[6, 1].Value = 2021;
cells[7, 1].Value = 2021;
cells[8, 1].Value = 2021;

cells[0, 2].Value = "amount";
cells[1, 2].Value = 50;
cells[2, 2].Value = 60;
cells[3, 2].Value = 70;
cells[4, 2].Value = 80;
cells[5, 2].Value = 90;
cells[6, 2].Value = 100;
cells[7, 2].Value = 110;
cells[8, 2].Value = 120;

PivotTableCollection pivots = sheet.PivotTables;

int pivotIndex = pivots.Add("=Sheet1!A1:C9", "A12", "TestPivotTable");
PivotTable pivot = pivots[pivotIndex];
pivot.AddFieldToArea(PivotFieldType.Row, "fruit");
pivot.AddFieldToArea(PivotFieldType.Column, "year");
pivot.AddFieldToArea(PivotFieldType.Data, "amount");

pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;
pivot.RefreshData();
pivot.CalculateData();

SlicerCollection slicers = sheet.Slicers;

int tableIndex = sheet.ListObjects.Add("A1", "C9", true);
ListObject table = sheet.ListObjects[tableIndex];

 //做你的事

book.Save("out.xlsx");

[Visual Basic]

Dim book As Workbook = New Workbook()
Dim sheet As Worksheet = book.Worksheets(0)
Dim cells As Cells = sheet.Cells

cells(0, 0).Value = "fruit"
cells(1, 0).Value = "grape"
cells(2, 0).Value = "blueberry"
cells(3, 0).Value = "kiwi"
cells(4, 0).Value = "cherry"
cells(5, 0).Value = "grape"
cells(6, 0).Value = "blueberry"
cells(7, 0).Value = "kiwi"
cells(8, 0).Value = "cherry"

cells(0, 1).Value = "year"
cells(1, 1).Value = 2020
cells(2, 1).Value = 2020
cells(3, 1).Value = 2020
cells(4, 1).Value = 2020
cells(5, 1).Value = 2021
cells(6, 1).Value = 2021
cells(7, 1).Value = 2021
cells(8, 1).Value = 2021

cells(0, 2).Value = "amount"
cells(1, 2).Value = 50
cells(2, 2).Value = 60
cells(3, 2).Value = 70
cells(4, 2).Value = 80
cells(5, 2).Value = 90
cells(6, 2).Value = 100
cells(7, 2).Value = 110
cells(8, 2).Value = 120

Dim pivots As PivotTableCollection = sheet.PivotTables
Dim pivotIndex As Int32 = pivots.Add("=Sheet1!A1:C9", "A12", "TestPivotTable")
Dim pivot As PivotTable = pivots(pivotIndex)
pivot.AddFieldToArea(PivotFieldType.Row, "fruit")
Pivot.AddFieldToArea(PivotFieldType.Column, "year")
Pivot.AddFieldToArea(PivotFieldType.Data, "amount")

pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10
pivot.RefreshData()
pivot.CalculateData()

Dim slicers As SlicerCollection = sheet.Slicers

Dim tableIndex As Int32 = sheet.ListObjects.Add("A1", "C9", True)
Dim table As ListObject = sheet.ListObjects(tableIndex)

book.Save("out_vb.xlsx")
```

### 也可以看看

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1)
* class [Slicer](../slicer)
* 命名空间 [Aspose.Cells.Slicers](../../aspose.cells.slicers)
* 部件 [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
