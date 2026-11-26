---
title: "CommentShape.Comment"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство CommentShape. Получает объект комментария"
type: docs
url: /ru/net/aspose.cells.drawing/commentshape/comment/
---
## CommentShape.Comment property

Получает объект комментария.

```csharp
public Comment Comment { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class CommentShapePropertyCommentDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить комментарий к ячейке A1
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            comment.Note = "This is a sample comment";
            
            // Получите форму комментария и продемонстрируйте свойство Comment
            CommentShape commentShape = worksheet.Comments[commentIndex].CommentShape;
            Comment retrievedComment = commentShape.Comment;
            
            // Отобразите текст комментария
            Console.WriteLine("Comment Text: " + retrievedComment.Note);
        }
    }
}
```

### См. также

* class [Comment](../../../aspose.cells/comment/)
* class [CommentShape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


