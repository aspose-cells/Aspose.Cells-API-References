---
title: "Класс ProtectedRangeCollection"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.ProtectedRangeCollection. Инкапсулирует коллекцию объектов ProtectedRange"
type: docs
url: /ru/net/aspose.cells/protectedrangecollection/
---
## ProtectedRangeCollection class

Инкапсулирует коллекцию объектов [`ProtectedRange`](../protectedrange/).

```csharp
public class ProtectedRangeCollection : CollectionBase<ProtectedRange>
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells/protectedrangecollection/item/) { get; } | Получает элемент [`ProtectedRange`](../protectedrange/) по указанному индексу. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Методы

| Имя | Описание |
| --- | --- |
| [Add](../../aspose.cells/protectedrangecollection/add/)(string, int, int, int, int) | Добавляет элемент [`ProtectedRange`](../protectedrange/) в коллекцию. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(ProtectedRange) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(ProtectedRange, IComparer&lt;ProtectedRange&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, ProtectedRange, IComparer&lt;ProtectedRange&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(ProtectedRange) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(ProtectedRange[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(ProtectedRange[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, ProtectedRange[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;ProtectedRange&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;ProtectedRange&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;ProtectedRange&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;ProtectedRange&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;ProtectedRange&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;ProtectedRange&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;ProtectedRange&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;ProtectedRange&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;ProtectedRange&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;ProtectedRange&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(ProtectedRange) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(ProtectedRange, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(ProtectedRange, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(ProtectedRange) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(ProtectedRange, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(ProtectedRange, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassProtectedRangeCollectionDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Получить коллекцию защищённых диапазонов
            ProtectedRangeCollection protectedRanges = worksheet.AllowEditRanges;

            // Добавить новый защищённый диапазон
            int index = protectedRanges.Add("MyProtectedRange", 0, 0, 2, 2);
            ProtectedRange protectedRange = protectedRanges[index];
            protectedRange.Password = "1234";

            // Добавить ещё один защищённый диапазон
            index = protectedRanges.Add("AnotherRange", 3, 3, 5, 5);
            protectedRange = protectedRanges[index];
            protectedRange.Password = "5678";

            // Отобразить информацию о защищённых диапазонах
            Console.WriteLine("Protected Ranges in Worksheet:");
            foreach (ProtectedRange range in protectedRanges)
            {
                Console.WriteLine($"Name: {range.Name}");
                Console.WriteLine($"Area: {range.CellArea.StartRow},{range.CellArea.StartColumn} to {range.CellArea.EndRow},{range.CellArea.EndColumn}");
                Console.WriteLine($"Password Protected: {!string.IsNullOrEmpty(range.Password)}");
                Console.WriteLine();
            }

            // Сохраните книгу
            workbook.Save("ProtectedRangesDemo.xlsx");
        }
    }
}
```

### См. также

* class [CollectionBase&lt;T&gt;](../collectionbase-1/)
* class [ProtectedRange](../protectedrange/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


