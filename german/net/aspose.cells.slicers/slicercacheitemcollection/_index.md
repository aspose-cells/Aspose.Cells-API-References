---
title: SlicerCacheItemCollection
second_title: Aspose.Cells für .NET-API-Referenz
description: Repräsentiert die Sammlung von SlicerCacheItem
type: docs
weight: 5670
url: /de/net/aspose.cells.slicers/slicercacheitemcollection/
---
## SlicerCacheItemCollection class

Repräsentiert die Sammlung von SlicerCacheItem

```csharp
public class SlicerCacheItemCollection : CollectionBase<SlicerCacheItem>
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase`1/capacity) { get; set; } |  |
| [Count](../../aspose.cells.slicers/slicercacheitemcollection/count) { get; } | Ruft die Anzahl der SlicerCacheItem ab. |
| [Item](../../aspose.cells.slicers/slicercacheitemcollection/item) { get; } | Ruft das SlicerCacheItem-Objekt nach Index ab. |
| [Item](../../aspose.cells/collectionbase`1/item) { get; set; } |  |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(SlicerCacheItem) |  |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(SlicerCacheItem, IComparer&lt;SlicerCacheItem&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(int, int, SlicerCacheItem, IComparer&lt;SlicerCacheItem&gt;) |  |
| [Clear](../../aspose.cells/collectionbase`1/clear)() |  |
| [Contains](../../aspose.cells/collectionbase`1/contains)(SlicerCacheItem) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(SlicerCacheItem[]) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(SlicerCacheItem[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(int, SlicerCacheItem[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase`1/exists)(Predicate&lt;SlicerCacheItem&gt;) |  |
| [Find](../../aspose.cells/collectionbase`1/find)(Predicate&lt;SlicerCacheItem&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase`1/findall)(Predicate&lt;SlicerCacheItem&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(Predicate&lt;SlicerCacheItem&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(int, Predicate&lt;SlicerCacheItem&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(int, int, Predicate&lt;SlicerCacheItem&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase`1/findlast)(Predicate&lt;SlicerCacheItem&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(Predicate&lt;SlicerCacheItem&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(int, Predicate&lt;SlicerCacheItem&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(int, int, Predicate&lt;SlicerCacheItem&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase`1/getenumerator)() |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(SlicerCacheItem) |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(SlicerCacheItem, int) |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(SlicerCacheItem, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(SlicerCacheItem) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(SlicerCacheItem, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(SlicerCacheItem, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase`1/removeat)(int) |  |

### Beispiele

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
int slicerIndex = slicers.Add(pivot, "E12", "fruit");
Slicer slicer = slicers[slicerIndex];
slicer.StyleType = SlicerStyleType.SlicerStyleLight2;

SlicerCacheItemCollection items = slicer.SlicerCache.SlicerCacheItems;
// Mach dein Geschäft
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
Dim slicerIndex As Int32 = slicers.Add(pivot, "E12", "fruit")
Dim slicer As Slicer = slicers(slicerIndex)
slicer.StyleType = SlicerStyleType.SlicerStyleLight2

Dim items As SlicerCacheItemCollection = slicer.SlicerCache.SlicerCacheItems

book.Save("out_vb.xlsx")
```

### Siehe auch

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1)
* class [SlicerCacheItem](../slicercacheitem)
* namensraum [Aspose.Cells.Slicers](../../aspose.cells.slicers)
* Montage [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
