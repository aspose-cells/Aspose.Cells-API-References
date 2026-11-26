---
title: "ThreadedCommentCollection.Item"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ThreadedCommentCollection. Получает ветвистый комментарий по указанному индексу"
type: docs
url: /ru/net/aspose.cells/threadedcommentcollection/item/
---
## ThreadedCommentCollection indexer

Получает цепочный комментарий по указанному индексу.

```csharp
public ThreadedComment this[int index] { get; }
```

| Параметр | Описание |
| --- | --- |
| индекс | Индекс |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ThreadedCommentCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить комментарий
            Comment comment = worksheet.Comments[worksheet.Comments.Add("A1")];
            comment.Note = "Initial comment";

            // Добавить цепочные комментарии
            ThreadedCommentCollection threadedComments = comment.ThreadedComments;
            ThreadedCommentAuthorCollection authors = workbook.Worksheets.ThreadedCommentAuthors;
            
            // Добавить авторов
            int author1Index = authors.Add("User1", "user1@example.com", "ID1");
            int author2Index = authors.Add("User2", "user2@example.com", "ID2");

            // Добавить цепочные комментарии
            threadedComments.Add("Reply 1", authors[author1Index]);
            threadedComments.Add("Reply 2", authors[author2Index]);

            // Продемонстрировать использование свойства Item
            ThreadedComment firstComment = threadedComments[0];
            ThreadedComment secondComment = threadedComments[1];

            Console.WriteLine("First comment author: " + firstComment.Author.Name);
            Console.WriteLine("Second comment author: " + secondComment.Author.Name);

            // Изменить автора второго комментария
            secondComment.Author = authors[author1Index];
            Console.WriteLine("Updated second comment author: " + secondComment.Author.Name);

            // Сохраните книгу
            workbook.Save("ThreadedCommentsDemo.xlsx");
        }
    }
}
```

### См. также

* class [ThreadedComment](../../threadedcomment/)
* class [ThreadedCommentCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


