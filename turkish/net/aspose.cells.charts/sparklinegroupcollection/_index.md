---
title: SparklineGroupCollection
second_title: Aspose.Cells for .NET API Referansı
description: Bir koleksiyonu kapsüllerSparklineGroup./sparklinegroup nesneler.
type: docs
weight: 890
url: /tr/net/aspose.cells.charts/sparklinegroupcollection/
---
## SparklineGroupCollection class

Bir koleksiyonu kapsüller[`SparklineGroup`](../sparklinegroup) nesneler.

```csharp
public class SparklineGroupCollection : CollectionBase<SparklineGroup>
```

## Özellikleri

| İsim | Tanım |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase`1/capacity) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase`1/count) { get; } |  |
| [Item](../../aspose.cells.charts/sparklinegroupcollection/item) { get; } | [`SparklineGroup`](../sparklinegroup) belirtilen dizindeki öğe. |
| [Item](../../aspose.cells/collectionbase`1/item) { get; set; } |  |

## yöntemler

| İsim | Tanım |
| --- | --- |
| [Add](../../aspose.cells.charts/sparklinegroupcollection/add)(SparklineType, string, bool, CellArea) | Bir[`SparklineGroup`](../sparklinegroup) koleksiyona öğe. |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(SparklineGroup) |  |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(SparklineGroup, IComparer&lt;SparklineGroup&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(int, int, SparklineGroup, IComparer&lt;SparklineGroup&gt;) |  |
| [Clear](../../aspose.cells/collectionbase`1/clear)() |  |
| [ClearSparklineGroups](../../aspose.cells.charts/sparklinegroupcollection/clearsparklinegroups)(CellArea) | Bir hücre alanıyla örtüşen mini grafik gruplarını temizler. |
| [ClearSparklines](../../aspose.cells.charts/sparklinegroupcollection/clearsparklines)(CellArea) | Bir hücre alanı içindeki mini grafikleri temizler. |
| [Contains](../../aspose.cells/collectionbase`1/contains)(SparklineGroup) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(SparklineGroup[]) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(SparklineGroup[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(int, SparklineGroup[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase`1/exists)(Predicate&lt;SparklineGroup&gt;) |  |
| [Find](../../aspose.cells/collectionbase`1/find)(Predicate&lt;SparklineGroup&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase`1/findall)(Predicate&lt;SparklineGroup&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(Predicate&lt;SparklineGroup&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(int, Predicate&lt;SparklineGroup&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(int, int, Predicate&lt;SparklineGroup&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase`1/findlast)(Predicate&lt;SparklineGroup&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(Predicate&lt;SparklineGroup&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(int, Predicate&lt;SparklineGroup&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(int, int, Predicate&lt;SparklineGroup&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase`1/getenumerator)() |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(SparklineGroup) |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(SparklineGroup, int) |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(SparklineGroup, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(SparklineGroup) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(SparklineGroup, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(SparklineGroup, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase`1/removeat)(int) |  |

### Örnekler

```csharp

[C#]
Workbook book = new Workbook(); 
Worksheet sheet = book.Worksheets[0];

sheet.Cells["A1"].PutValue(5);
sheet.Cells["B1"].PutValue(2);
sheet.Cells["C1"].PutValue(1);
sheet.Cells["D1"].PutValue(3);

// CellArea'yı tanımlayın
CellArea ca = new CellArea();
ca.StartColumn = 4;
ca.EndColumn = 4;
ca.StartRow = 0;
ca.EndRow = 0;

int idx = sheet.SparklineGroupCollection.Add(Aspose.Cells.Charts.SparklineType.Line, "A1:D1", false, ca);
SparklineGroup group = sheet.SparklineGroupCollection[idx];
group.SparklineCollection.Add(sheet.Name + "!A1:D1", 0, 4);
book.Save("output.xlsx", SaveFormat.Xlsx);
```

### Ayrıca bakınız

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1)
* class [SparklineGroup](../sparklinegroup)
* ad alanı [Aspose.Cells.Charts](../../aspose.cells.charts)
* toplantı [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
