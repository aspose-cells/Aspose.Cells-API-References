---
title: "ThreadedComment.CreatedTime"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ThreadedComment. Получает и задает время создания этого цепочного комментария"
type: docs
url: /ru/net/aspose.cells/threadedcomment/createdtime/
---
## ThreadedComment.CreatedTime property

Получает и задаёт время создания этого ветвлёного комментария.

```csharp
public DateTime CreatedTime { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ThreadedCommentPropertyCreatedTimeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Создайте автора цепочного комментария
            ThreadedCommentAuthor author = workbook.Worksheets.ThreadedCommentAuthors["User1"];
            
            // Добавить комментарий к ячейке A1
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            
            // Добавить ветвящийся комментарий
            int threadedCommentIndex = comment.ThreadedComments.Add("Test comment", author);
            ThreadedComment threadedComment = comment.ThreadedComments[threadedCommentIndex];
            
            // Продемонстрируйте свойство CreatedTime
            Console.WriteLine("Threaded comment created at: " + threadedComment.CreatedTime);
            
            // Сохраните книгу
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [ThreadedComment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


