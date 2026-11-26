---
title: "Класс CellWatchCollection"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.CellWatchCollection. Представляет коллекцию ячеек этого листа, наблюдаемых в окне наблюдения."
type: docs
url: /ru/net/aspose.cells/cellwatchcollection/
---
## CellWatchCollection class

Представляет коллекцию ячеек этого листа, наблюдаемых в 'watch window'.

```csharp
public class CellWatchCollection : CollectionBase<CellWatch>
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [CellWatchCollection](cellwatchcollection/)() | Конструктор по умолчанию. |

## Свойства

| Имя | Описание |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells/cellwatchcollection/item/) { get; } | Получает и задает [`CellWatch`](../cellwatch/) по индексу. (2 индексатора) |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Методы

| Имя | Описание |
| --- | --- |
| [Add](../../aspose.cells/cellwatchcollection/add/#add_1)(string) | Добавляет [`CellWatch`](../cellwatch/) с именем ячейки. |
| [Add](../../aspose.cells/cellwatchcollection/add/#add)(int, int) | Добавляет [`CellWatch`](../cellwatch/) с строкой и столбцом. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(CellWatch) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(CellWatch, IComparer&lt;CellWatch&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, CellWatch, IComparer&lt;CellWatch&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(CellWatch) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(CellWatch[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(CellWatch[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, CellWatch[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;CellWatch&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;CellWatch&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;CellWatch&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;CellWatch&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;CellWatch&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;CellWatch&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;CellWatch&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;CellWatch&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;CellWatch&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;CellWatch&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(CellWatch) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(CellWatch, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(CellWatch, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(CellWatch) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(CellWatch, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(CellWatch, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellWatchCollectionDemo
    {
        public static void CellWatchCollectionExample()
        {
            // Создание объекта Workbook
            Workbook workbook = new Workbook();
            
            // Получить первый Worksheet
            Worksheet sheet = workbook.Worksheets[0];
            
            // Добавить элемент наблюдения за ячейкой в окно наблюдения
            int watchIndex = sheet.CellWatches.Add("B2");
            
            // Получить доступ к CellWatchCollection
            CellWatchCollection cellWatches = sheet.CellWatches;
            
            // Получить доступ к добавленному элементу CellWatch
            CellWatch cellWatch = cellWatches[watchIndex];
            
            // Отобразить свойства элемента CellWatch
            Console.WriteLine("Cell Watch Details:");
            Console.WriteLine($"Row: {cellWatch.Row}");
            Console.WriteLine($"Column: {cellWatch.Column}");
            Console.WriteLine($"Cell Name: {cellWatch.CellName}");
            
            // Изменить свойства элемента CellWatch
            cellWatch.Row = 1;
            cellWatch.Column = 1;
            cellWatch.CellName = "A2";
            
            // Отобразить изменённые свойства элемента CellWatch
            Console.WriteLine("Modified Cell Watch Details:");
            Console.WriteLine($"Row: {cellWatch.Row}");
            Console.WriteLine($"Column: {cellWatch.Column}");
            Console.WriteLine($"Cell Name: {cellWatch.CellName}");
            
            // Сохраните книгу
            workbook.Save("CellWatchCollectionExample.xlsx");
            workbook.Save("CellWatchCollectionExample.pdf");
        }
    }
}
```

### См. также

* class [CollectionBase&lt;T&gt;](../collectionbase-1/)
* class [CellWatch](../cellwatch/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


