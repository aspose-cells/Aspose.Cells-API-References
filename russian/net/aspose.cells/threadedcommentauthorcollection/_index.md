---
title: "Класс ThreadedCommentAuthorCollection"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.ThreadedCommentAuthorCollection. Представляет всех участников"
type: docs
url: /ru/net/aspose.cells/threadedcommentauthorcollection/
---
## ThreadedCommentAuthorCollection class

Представляет всех лиц.

```csharp
public class ThreadedCommentAuthorCollection : CollectionBase<ThreadedCommentAuthor>
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [ThreadedCommentAuthorCollection](threadedcommentauthorcollection/)() | Конструктор по умолчанию. |

## Свойства

| Имя | Описание |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [CurrentPerson](../../aspose.cells/threadedcommentauthorcollection/currentperson/) { get; set; } | Получает и задает текущего пользователя. |
| [Item](../../aspose.cells/threadedcommentauthorcollection/item/) { get; } | Получает лицо, создающее цепочечные комментарии. (2 индексатора) |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Методы

| Имя | Описание |
| --- | --- |
| [Add](../../aspose.cells/threadedcommentauthorcollection/add/)(string, string, string) | Добавляет одного участника цепочечного комментария. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(ThreadedCommentAuthor) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(ThreadedCommentAuthor, IComparer&lt;ThreadedCommentAuthor&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, ThreadedCommentAuthor, IComparer&lt;ThreadedCommentAuthor&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(ThreadedCommentAuthor) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(ThreadedCommentAuthor[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(ThreadedCommentAuthor[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, ThreadedCommentAuthor[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;ThreadedCommentAuthor&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;ThreadedCommentAuthor&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;ThreadedCommentAuthor&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;ThreadedCommentAuthor&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;ThreadedCommentAuthor&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;ThreadedCommentAuthor&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;ThreadedCommentAuthor&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;ThreadedCommentAuthor&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;ThreadedCommentAuthor&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;ThreadedCommentAuthor&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/threadedcommentauthorcollection/indexof/#indexof)(ThreadedCommentAuthor) | Получает индекс объекта ThreadedCommentAuthor (2 метода) |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(ThreadedCommentAuthor, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(ThreadedCommentAuthor, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(ThreadedCommentAuthor) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(ThreadedCommentAuthor, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(ThreadedCommentAuthor, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ThreadedCommentAuthorCollectionDemo
    {
        public static void ThreadedCommentAuthorCollectionExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Доступ к ThreadedCommentAuthorCollection
            ThreadedCommentAuthorCollection authors = workbook.Worksheets.ThreadedCommentAuthors;

            // Добавить нового автора цепочечного комментария
            int authorIndex = authors.Add("John Doe", "john.doe@example.com", "providerId123");

            // Получить добавленного автора
            ThreadedCommentAuthor author = authors[authorIndex];

            // Установить текущего человека
            authors.CurrentPerson = author;

            // Отобразить детали текущего человека
            Console.WriteLine("Current Person: " + authors.CurrentPerson.Name);

            // Сохраните книгу
            workbook.Save("ThreadedCommentAuthorCollectionExample.xlsx");

            return;
        }
    }
}
```

### См. также

* class [CollectionBase&lt;T&gt;](../collectionbase-1/)
* class [ThreadedCommentAuthor](../threadedcommentauthor/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


