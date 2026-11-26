---
title: "Класс HyperlinkCollection"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.HyperlinkCollection. Инкапсулирует коллекцию объектов Hyperlink."
type: docs
url: /ru/net/aspose.cells/hyperlinkcollection/
---
## HyperlinkCollection class

Инкапсулирует коллекцию объектов [`Hyperlink`](../hyperlink/).

```csharp
public class HyperlinkCollection : CollectionBase<Hyperlink>
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells/hyperlinkcollection/item/) { get; } | Получает элемент [`Hyperlink`](../hyperlink/) по указанному индексу. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Методы

| Имя | Описание |
| --- | --- |
| [Add](../../aspose.cells/hyperlinkcollection/add/#add_1)(string, int, int, string) | Добавляет гиперссылку в указанную ячейку или диапазон ячеек. |
| [Add](../../aspose.cells/hyperlinkcollection/add/#add)(int, int, int, int, string) | Добавляет гиперссылку в указанную ячейку или диапазон ячеек. |
| [Add](../../aspose.cells/hyperlinkcollection/add/#add_2)(string, string, string, string, string) | Добавляет гиперссылку в указанную ячейку или диапазон ячеек. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(Hyperlink) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(Hyperlink, IComparer&lt;Hyperlink&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, Hyperlink, IComparer&lt;Hyperlink&gt;) |  |
| [Clear](../../aspose.cells/hyperlinkcollection/clear/#clear)() | Очищает все гиперссылки. (2 метода) |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(Hyperlink) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(Hyperlink[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(Hyperlink[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, Hyperlink[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;Hyperlink&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;Hyperlink&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;Hyperlink&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;Hyperlink&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;Hyperlink&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;Hyperlink&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;Hyperlink&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;Hyperlink&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;Hyperlink&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;Hyperlink&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Hyperlink) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Hyperlink, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Hyperlink, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Hyperlink) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Hyperlink, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Hyperlink, int, int) |  |
| [RemoveAt](../../aspose.cells/hyperlinkcollection/removeat/#removeat)(int) | Удаляет гиперссылку по указанному индексу в этой коллекции. (2 метода) |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class HyperlinkCollectionDemo
    {
        public static void HyperlinkCollectionExample()
        {
            // Создание объекта Workbook
            Workbook workbook = new Workbook();

            // Получение ссылки на только что добавленный лист путем передачи его индекса листа
            Worksheet worksheet = workbook.Worksheets[0];

            // Получить коллекцию гиперссылок
            HyperlinkCollection hyperlinks = worksheet.Hyperlinks;

            // Добавление гиперссылки на URL в ячейку "A1"
            hyperlinks.Add("A1", 1, 1, "http://www.aspose.com");

            // Добавление еще одной гиперссылки на URL в ячейку "B1"
            hyperlinks.Add("B1", 1, 1, "http://www.example.com");

            // Добавление гиперссылки с диапазоном ячеек
            hyperlinks.Add("C1", 1, 2, "http://www.test.com");

            // Добавление гиперссылки с определённым текстом для отображения и подсказкой
            hyperlinks.Add("D1", "D2", "http://www.display.com", "Click Here", "Go to Display");

            // Удаление первой гиперссылки
            hyperlinks.RemoveAt(0);

            // Очистка всех гиперссылок
            hyperlinks.Clear();

            // Повторное добавление гиперссылки для демонстрации сохранения
            hyperlinks.Add("A1", 1, 1, "http://www.aspose.com");

            // Сохранение файла Excel
            workbook.Save("HyperlinkCollectionExample.xlsx");
            workbook.Save("HyperlinkCollectionExample.pdf");
            return;
        }
    }
}
```

### См. также

* class [CollectionBase&lt;T&gt;](../collectionbase-1/)
* class [Hyperlink](../hyperlink/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


