---
title: "Comment.Font"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Comment. Получает шрифт комментария"
type: docs
url: /ru/net/aspose.cells/comment/font/
---
## Comment.Font property

Получает шрифт комментария.

```csharp
public Font Font { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentPropertyFontDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить комментарий к ячейке A1
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            comment.Note = "Sample comment";

            // Получить доступ и изменить свойства шрифта комментария
            Aspose.Cells.Font font = comment.Font;
            font.Size = 12;
            font.Name = "Arial";
            font.Color = System.Drawing.Color.Red;
            font.IsBold = true;

            // Сохраните книгу
            workbook.Save("CommentFontDemo.xlsx");
        }
    }
}
```

### См. также

* class [Font](../../font/)
* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


