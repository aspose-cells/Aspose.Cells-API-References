---
title: CellWatchCollection
second_title: Aspose.Cells för .NET API-referens
description: Representerar samlingen av celler på detta kalkylblad som bevakas i bevakningsfönstret.
type: docs
weight: 290
url: /sv/net/aspose.cells/cellwatchcollection/
---
## CellWatchCollection class

Representerar samlingen av celler på detta kalkylblad som bevakas i "bevakningsfönstret".

```csharp
public class CellWatchCollection : CollectionBase<CellWatch>
```

## Konstruktörer

| namn | Beskrivning |
| --- | --- |
| [CellWatchCollection](cellwatchcollection)() | Default_Constructor |

## Egenskaper

| namn | Beskrivning |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase`1/capacity) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase`1/count) { get; } |  |
| [Item](../../aspose.cells/cellwatchcollection/item) { get; } | Hämtar och ställer[`CellWatch`](../cellwatch) efter index. (2 indexers) |
| [Item](../../aspose.cells/collectionbase`1/item) { get; set; } |  |

## Metoder

| namn | Beskrivning |
| --- | --- |
| [Add](../../aspose.cells/cellwatchcollection/add#add_1)(string) | Lägger till |
| [Add](../../aspose.cells/cellwatchcollection/add#add)(int, int) | Lägger till[`CellWatch`](../cellwatch) med rad och kolumn. |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(CellWatch) |  |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(CellWatch, IComparer&lt;CellWatch&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(int, int, CellWatch, IComparer&lt;CellWatch&gt;) |  |
| [Clear](../../aspose.cells/collectionbase`1/clear)() |  |
| [Contains](../../aspose.cells/collectionbase`1/contains)(CellWatch) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(CellWatch[]) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(CellWatch[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(int, CellWatch[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase`1/exists)(Predicate&lt;CellWatch&gt;) |  |
| [Find](../../aspose.cells/collectionbase`1/find)(Predicate&lt;CellWatch&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase`1/findall)(Predicate&lt;CellWatch&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(Predicate&lt;CellWatch&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(int, Predicate&lt;CellWatch&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(int, int, Predicate&lt;CellWatch&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase`1/findlast)(Predicate&lt;CellWatch&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(Predicate&lt;CellWatch&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(int, Predicate&lt;CellWatch&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(int, int, Predicate&lt;CellWatch&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase`1/getenumerator)() |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(CellWatch) |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(CellWatch, int) |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(CellWatch, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(CellWatch) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(CellWatch, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(CellWatch, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase`1/removeat)(int) |  |

### Exempel

```csharp

[C#]

//Instantiering av ett arbetsboksobjekt
Workbook workbook = new Workbook();
// Skaffa det första arbetsbladet.
Worksheet sheet = workbook.Worksheets[0];
// Lägg till cellbevakningsobjekt i bevakningsfönstret
sheet.CellWatches.Add("B2");

 [Visual Basic]

'Instantiera ett arbetsboksobjekt
Dim workbook As Workbook = New Workbook()
'Skaffa det första arbetsbladet.
Dim sheet as Worksheet = workbook.Worksheets(0);
'Lägg till cellbevakningsobjekt i bevakningsfönstret
sheet.CellWatches.Add("B2")
```

### Se även

* class [CollectionBase&lt;T&gt;](../collectionbase-1)
* class [CellWatch](../cellwatch)
* namnutrymme [Aspose.Cells](../../aspose.cells)
* hopsättning [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
