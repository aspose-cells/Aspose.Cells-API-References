---
title: "Класс ThreadedCommentAuthor"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.ThreadedCommentAuthor. Представляет лицо, создающее цепочечные комментарии"
type: docs
url: /ru/net/aspose.cells/threadedcommentauthor/
---
## ThreadedCommentAuthor class

Представляет лицо, создающее вложенные комментарии.

```csharp
public class ThreadedCommentAuthor
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Name](../../aspose.cells/threadedcommentauthor/name/) { get; set; } | Получает и задает имя. |
| [ProviderId](../../aspose.cells/threadedcommentauthor/providerid/) { get; set; } | Получает идентификатор поставщика. |
| [UserId](../../aspose.cells/threadedcommentauthor/userid/) { get; set; } | Получает и задает идентификатор пользователя. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassThreadedCommentAuthorDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить комментарий
            int commentIndex = worksheet.Comments.Add("C1");
            Comment comment = worksheet.Comments[commentIndex];
            comment.Note = "Initial comment";
            
            // Добавить авторов ветвящихся комментариев
            int authorIndex1 = workbook.Worksheets.ThreadedCommentAuthors.Add("Author1", "user1", "");
            ThreadedCommentAuthor author1 = workbook.Worksheets.ThreadedCommentAuthors[authorIndex1];
            
            // Добавить ветвящийся комментарий
            int threadedCommentIndex = comment.ThreadedComments.Add("Threaded comment text", author1);
            ThreadedComment threadedComment = comment.ThreadedComments[threadedCommentIndex];
            
            // Получить доступ и изменить автора
            Console.WriteLine("Original author: " + threadedComment.Author.Name);
            threadedComment.Author.Name = "ModifiedAuthor";
            Console.WriteLine("Modified author: " + threadedComment.Author.Name);

            // Создать нового автора и назначить его
            int authorIndex2 = workbook.Worksheets.ThreadedCommentAuthors.Add("Author2", "user2", "");
            ThreadedCommentAuthor author2 = workbook.Worksheets.ThreadedCommentAuthors[authorIndex2];
            threadedComment.Author = author2;
            Console.WriteLine("New author: " + threadedComment.Author.Name);
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


