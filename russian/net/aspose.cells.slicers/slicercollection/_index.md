---
title: SlicerCollection
second_title: Справочник по Aspose.Cells для .NET API
description: Задает набор всех объектов Slicer на указанном рабочем листе.
type: docs
weight: 5690
url: /ru/net/aspose.cells.slicers/slicercollection/
---
## SlicerCollection class

Задает набор всех объектов Slicer на указанном рабочем листе.

```csharp
public class SlicerCollection : CollectionBase<Slicer>
```

## Характеристики

| Имя | Описание |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase`1/capacity) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase`1/count) { get; } |  |
| [Item](../../aspose.cells.slicers/slicercollection/item) { get; } | Получает слайсер по индексу. (2 indexers) |
| [Item](../../aspose.cells/collectionbase`1/item) { get; set; } |  |

## Методы

| Имя | Описание |
| --- | --- |
| [Add](../../aspose.cells.slicers/slicercollection/add#add_8)(ListObject, int, string) | Добавить новый слайсер, используя ListObjet в качестве источника данных |
| [Add](../../aspose.cells.slicers/slicercollection/add#add_7)(ListObject, ListColumn, string) | Добавить новый слайсер, используя ListObjet в качестве источника данных |
| [Add](../../aspose.cells.slicers/slicercollection/add#add_4)(PivotTable, string, int) | Добавить новый слайсер, используя сводную таблицу в качестве источника данных |
| [Add](../../aspose.cells.slicers/slicercollection/add#add_3)(PivotTable, string, PivotField) | Добавить новый слайсер, используя сводную таблицу в качестве источника данных |
| [Add](../../aspose.cells.slicers/slicercollection/add#add_5)(PivotTable, string, string) | Добавить новый слайсер, используя сводную таблицу в качестве источника данных |
| [Add](../../aspose.cells.slicers/slicercollection/add#add_6)(ListObject, ListColumn, int, int) | Добавить новый слайсер, используя ListObjet в качестве источника данных |
| [Add](../../aspose.cells.slicers/slicercollection/add#add_1)(PivotTable, int, int, int) | Добавить новый слайсер, используя сводную таблицу в качестве источника данных |
| [Add](../../aspose.cells.slicers/slicercollection/add#add)(PivotTable, int, int, PivotField) | Добавить новый слайсер, используя сводную таблицу в качестве источника данных |
| [Add](../../aspose.cells.slicers/slicercollection/add#add_2)(PivotTable, int, int, string) | Добавить новый слайсер, используя сводную таблицу в качестве источника данных |
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
| [Remove](../../aspose.cells.slicers/slicercollection/remove)(Slicer) | Удалить указанный слайсер |
| [RemoveAt](../../aspose.cells.slicers/slicercollection/removeat#removeat)(int) | Удаляет слайсер по указанному индексу (2 methods) |

### Примеры

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

  //делай свое дело

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

### Смотрите также

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1)
* class [Slicer](../slicer)
* пространство имен [Aspose.Cells.Slicers](../../aspose.cells.slicers)
* сборка [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
