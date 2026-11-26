---
title: "Класс HorizontalPageBreakCollection"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.HorizontalPageBreakCollection. Инкапсулирует коллекцию объектов HorizontalPageBreak"
type: docs
url: /ru/net/aspose.cells/horizontalpagebreakcollection/
---
## HorizontalPageBreakCollection class

Инкапсулирует коллекцию объектов [`HorizontalPageBreak`](../horizontalpagebreak/).

```csharp
public class HorizontalPageBreakCollection : CollectionBase<HorizontalPageBreak>
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells/horizontalpagebreakcollection/item/) { get; } | Получает элемент [`HorizontalPageBreak`](../horizontalpagebreak/) по указанному индексу. (2 индексатора) |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Методы

| Имя | Описание |
| --- | --- |
| [Add](../../aspose.cells/horizontalpagebreakcollection/add/#add)(int) | Добавляет горизонтальный разрыв страницы в коллекцию. |
| [Add](../../aspose.cells/horizontalpagebreakcollection/add/#add_3)(string) | Добавляет горизонтальный разрыв страницы в коллекцию. |
| [Add](../../aspose.cells/horizontalpagebreakcollection/add/#add_1)(int, int) | Добавляет горизонтальный разрыв страницы в коллекцию. |
| [Add](../../aspose.cells/horizontalpagebreakcollection/add/#add_2)(int, int, int) | Добавляет горизонтальный разрыв страницы в коллекцию. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(HorizontalPageBreak) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(HorizontalPageBreak, IComparer&lt;HorizontalPageBreak&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, HorizontalPageBreak, IComparer&lt;HorizontalPageBreak&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(HorizontalPageBreak) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(HorizontalPageBreak[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(HorizontalPageBreak[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, HorizontalPageBreak[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;HorizontalPageBreak&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;HorizontalPageBreak&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;HorizontalPageBreak&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;HorizontalPageBreak&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;HorizontalPageBreak&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;HorizontalPageBreak&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;HorizontalPageBreak&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;HorizontalPageBreak&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;HorizontalPageBreak&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;HorizontalPageBreak&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(HorizontalPageBreak) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(HorizontalPageBreak, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(HorizontalPageBreak, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(HorizontalPageBreak) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(HorizontalPageBreak, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(HorizontalPageBreak, int, int) |  |
| [RemoveAt](../../aspose.cells/horizontalpagebreakcollection/removeat/#removeat)(int) | Удаляет элемент HPageBreak по указанному имени. (2 метода) |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class HorizontalPageBreakCollectionDemo
    {
        public static void HorizontalPageBreakCollectionExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить горизонтальный разрыв страницы в строке 5
            worksheet.HorizontalPageBreaks.Add(5);
            
            // Добавить горизонтальный разрыв страницы в строке 10, начиная с колонки 1 до колонки 5
            worksheet.HorizontalPageBreaks.Add(10, 1, 5);
            
            // Добавить горизонтальный разрыв страницы в строке 15, начиная с колонки 2
            worksheet.HorizontalPageBreaks.Add(15, 2);
            
            // Добавить горизонтальный разрыв страницы в ячейке "G5"
            worksheet.HorizontalPageBreaks.Add("G5");
            
            // Удалить первый горизонтальный разрыв страницы
            worksheet.HorizontalPageBreaks.RemoveAt(0);
            
            // Сохраните книгу
            workbook.Save("HorizontalPageBreakCollectionExample.xlsx");
            workbook.Save("HorizontalPageBreakCollectionExample.pdf");
            return;
        }
    }
}
```

### См. также

* class [CollectionBase&lt;T&gt;](../collectionbase-1/)
* class [HorizontalPageBreak](../horizontalpagebreak/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


