---
title: "Класс ThreadedComment"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.ThreadedComment. Представляет ветвлёный комментарий"
type: docs
url: /ru/net/aspose.cells/threadedcomment/
---
## ThreadedComment class

Представляет вложенный комментарий.

```csharp
public class ThreadedComment
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Author](../../aspose.cells/threadedcomment/author/) { get; set; } | Получает автора комментария. |
| [Column](../../aspose.cells/threadedcomment/column/) { get; } | Получает индекс столбца комментария. |
| [CreatedTime](../../aspose.cells/threadedcomment/createdtime/) { get; set; } | Получает и задаёт время создания этого ветвлёного комментария. |
| [Notes](../../aspose.cells/threadedcomment/notes/) { get; set; } | Получает и задаёт текст комментария. |
| [Row](../../aspose.cells/threadedcomment/row/) { get; } | Получает индекс строки комментария. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassThreadedCommentDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте авторов в книгу
            int author1Id = workbook.Worksheets.ThreadedCommentAuthors.Add("User1", "user1@example.com", "1");
            int author2Id = workbook.Worksheets.ThreadedCommentAuthors.Add("User2", "", "2");
            
            // Получите ссылки на авторов
            ThreadedCommentAuthor author1 = workbook.Worksheets.ThreadedCommentAuthors[author1Id];
            ThreadedCommentAuthor author2 = workbook.Worksheets.ThreadedCommentAuthors[author2Id];
            
            // Добавить комментарий к ячейке A1
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            
            // Добавьте ветвлёный комментарий к комментарию
            int threadedCommentIndex = comment.ThreadedComments.Add("This is a threaded comment", author1);
            ThreadedComment threadedComment = comment.ThreadedComments[threadedCommentIndex];
            
            // Установить дополнительные свойства
            threadedComment.Notes = "Additional notes";
            
            // Добавьте ответ к ветвлённому комментарию
            int replyIndex = comment.ThreadedComments.Add("This is a reply", author2);
            ThreadedComment reply = comment.ThreadedComments[replyIndex];
            
            // Сохраните книгу
            workbook.Save("ThreadedCommentDemo.xlsx");
            
            Console.WriteLine("Threaded comment demo completed.");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


