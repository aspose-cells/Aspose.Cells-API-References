---
title: "Класс CommentCollection"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.CommentCollection. Инкапсулирует коллекцию объектов Comment"
type: docs
url: /ru/net/aspose.cells/commentcollection/
---
## CommentCollection class

Инкапсулирует коллекцию объектов [`Comment`](../comment/).

```csharp
public class CommentCollection : CollectionBase<Comment>
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells/commentcollection/item/) { get; } | Получает элемент [`Comment`](../comment/) по указанному индексу. (3 индексатора) |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Методы

| Имя | Описание |
| --- | --- |
| [Add](../../aspose.cells/commentcollection/add/#add_1)(string) | Добавляет комментарий в коллекцию. |
| [Add](../../aspose.cells/commentcollection/add/#add)(int, int) | Добавляет комментарий в коллекцию. |
| [AddThreadedComment](../../aspose.cells/commentcollection/addthreadedcomment/#addthreadedcomment_1)(string, string, ThreadedCommentAuthor) | Добавляет цепочный комментарий. |
| [AddThreadedComment](../../aspose.cells/commentcollection/addthreadedcomment/#addthreadedcomment)(int, int, string, ThreadedCommentAuthor) | Добавляет цепочный комментарий. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(Comment) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(Comment, IComparer&lt;Comment&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, Comment, IComparer&lt;Comment&gt;) |  |
| [Clear](../../aspose.cells/commentcollection/clear/#clear)() | Удаляет все комментарии; (2 метода) |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(Comment) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(Comment[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(Comment[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, Comment[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;Comment&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;Comment&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;Comment&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;Comment&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;Comment&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;Comment&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;Comment&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;Comment&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;Comment&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;Comment&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [GetThreadedComments](../../aspose.cells/commentcollection/getthreadedcomments/#getthreadedcomments_1)(string) | Получает ветвящиеся комментарии по имени ячейки. |
| [GetThreadedComments](../../aspose.cells/commentcollection/getthreadedcomments/#getthreadedcomments)(int, int) | Получает ветвящиеся комментарии по индексу строки и столбца. |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Comment) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Comment, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Comment, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Comment) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Comment, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Comment, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |
| [RemoveAt](../../aspose.cells/commentcollection/removeat/#removeat_2)(string) | Удаляет комментарий конкретной ячейки. |
| [RemoveAt](../../aspose.cells/commentcollection/removeat/#removeat_1)(int, int) | Удаляет комментарий конкретной ячейки. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CommentCollectionDemo
    {
        public static void CommentCollectionExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Получить доступ к коллекции комментариев листа
            CommentCollection comments = worksheet.Comments;

            // Добавить комментарий к ячейке A1
            int commentIndex1 = comments.Add(0, 0);
            Comment comment1 = comments[commentIndex1];
            comment1.Note = "First note.";
            comment1.Author = "Author1";
            comment1.Font.Name = "Times New Roman";

            // Добавить комментарий в ячейку B2
            comments.Add("B2");
            Comment comment2 = comments["B2"];
            comment2.Note = "Second note.";
            comment2.Author = "Author2";

            // Добавить ветвящийся комментарий в ячейку C3
            int authorIndex = workbook.Worksheets.ThreadedCommentAuthors.Add("Author3", "user3", "provider3");
            ThreadedCommentAuthor author = workbook.Worksheets.ThreadedCommentAuthors[authorIndex];
            comments.AddThreadedComment(2, 2, "This is a threaded comment.", author);

            // Получить ветвящиеся комментарии из ячейки C3
            var threadedComments = comments.GetThreadedComments(2, 2);
            foreach (var threadedComment in threadedComments)
            {
                Console.WriteLine(threadedComment.Notes);
            }

            // Удалить комментарий в ячейке A1
            comments.RemoveAt(0, 0);

            // Очистить все комментарии
            comments.Clear();

            // Сохраните книгу
            workbook.Save("CommentCollectionExample.xlsx");
            workbook.Save("CommentCollectionExample.pdf");
        }
    }
}
```

### См. также

* class [CollectionBase&lt;T&gt;](../collectionbase-1/)
* class [Comment](../comment/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


