---
title: "Comment.IsThreadedComment"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Comment. Указывает, является ли этот комментарий ветвистым."
type: docs
url: /ru/net/aspose.cells/comment/isthreadedcomment/
---
## Comment.IsThreadedComment property

Указывает, является ли этот комментарий ветвистым.

```csharp
public bool IsThreadedComment { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentPropertyIsThreadedCommentDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить обычный комментарий
            Comment regularComment = worksheet.Comments[worksheet.Comments.Add("A1")];
            regularComment.Note = "This is a regular comment";
            regularComment.Author = "User1";

            // Добавить ветвистый комментарий (при условии, что API поддерживает добавление ветвистых комментариев)
            Comment threadedComment = worksheet.Comments[worksheet.Comments.Add("B1")];
            threadedComment.Note = "This is a threaded comment";
            threadedComment.Author = "User2";

            // Проверить типы комментариев
            Console.WriteLine("Comment at A1 is threaded: " + regularComment.IsThreadedComment);
            Console.WriteLine("Comment at B1 is threaded: " + threadedComment.IsThreadedComment);

            // Обрабатывать комментарии в зависимости от их типа
            foreach (Comment comment in worksheet.Comments)
            {
                if (comment.IsThreadedComment)
                {
                    Console.WriteLine($"Threaded comment found at {CellsHelper.CellIndexToName(comment.Row, comment.Column)}");
                    Console.WriteLine($"Author: {comment.Author}, Note: {comment.Note}");
                }
                else
                {
                    Console.WriteLine($"Regular comment found at {CellsHelper.CellIndexToName(comment.Row, comment.Column)}");
                }
            }
        }
    }
}
```

### См. также

* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


