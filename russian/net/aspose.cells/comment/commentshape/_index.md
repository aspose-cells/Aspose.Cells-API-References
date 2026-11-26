---
title: "Comment.CommentShape"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Comment. Получить объект Shape, который представляет форму, прикреплённую к указанному комментарию"
type: docs
url: /ru/net/aspose.cells/comment/commentshape/
---
## Comment.CommentShape property

Получить объект Shape, представляющий форму, прикреплённую к указанному комментарию.

```csharp
public CommentShape CommentShape { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class CommentPropertyCommentShapeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить комментарий к ячейке A1
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment1 = worksheet.Comments[commentIndex];
            comment1.Note = "This is a sample comment";

            // Получить CommentShape и изменить его свойства
            Shape shape = comment1.CommentShape;
            shape.Width = 200;
            shape.Height = 100;
            shape.FillFormat.ForeColor = System.Drawing.Color.LightYellow;
            shape.LineFormat.ForeColor = System.Drawing.Color.Blue;

            // Отобразить размеры формы
            Console.WriteLine("Comment shape width: " + shape.Width);
            Console.WriteLine("Comment shape height: " + shape.Height);
        }
    }
}
```

### См. также

* class [CommentShape](../../../aspose.cells.drawing/commentshape/)
* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


