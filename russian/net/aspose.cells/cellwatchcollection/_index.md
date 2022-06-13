---
title: CellWatchCollection
second_title: Справочник по Aspose.Cells для .NET API
description: Представляет набор ячеек на этом рабочем листе наблюдаемых в окне просмотра.
type: docs
weight: 290
url: /ru/net/aspose.cells/cellwatchcollection/
---
## CellWatchCollection class

Представляет набор ячеек на этом рабочем листе, наблюдаемых в «окне просмотра».

```csharp
public class CellWatchCollection : CollectionBase<CellWatch>
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [CellWatchCollection](cellwatchcollection)() | Конструктор по умолчанию. |

## Характеристики

| Имя | Описание |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase`1/capacity) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase`1/count) { get; } |  |
| [Item](../../aspose.cells/cellwatchcollection/item) { get; } | Получает и устанавливает[`CellWatch`](../cellwatch)по индексу. (2 indexers) |
| [Item](../../aspose.cells/collectionbase`1/item) { get; set; } |  |

## Методы

| Имя | Описание |
| --- | --- |
| [Add](../../aspose.cells/cellwatchcollection/add#add_1)(string) | Добавляет |
| [Add](../../aspose.cells/cellwatchcollection/add#add)(int, int) | Добавляет[`CellWatch`](../cellwatch)со строкой и столбцом. |
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

### Примеры

```csharp

[C#]

  //Создание экземпляра рабочей книги object
Workbook workbook = new Workbook();
  // Получить первый рабочий лист.
Worksheet sheet = workbook.Worksheets[0];
  // Добавляем Cell Watch Item в Watch window
sheet.CellWatches.Add("B2");

 [Visual Basic]

'Instantiating a Workbook object
Dim workbook As Workbook = New Workbook()
'Get the first Worksheet.
Dim sheet as Worksheet = workbook.Worksheets(0);
'Add Cell Watch Item into the watch window
sheet.CellWatches.Add("B2")
```

### Смотрите также

* class [CollectionBase&lt;T&gt;](../collectionbase-1)
* class [CellWatch](../cellwatch)
* пространство имен [Aspose.Cells](../../aspose.cells)
* сборка [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->