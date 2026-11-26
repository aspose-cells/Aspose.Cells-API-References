---
title: "Comment.Width"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Comment. Представляет ширину комментария в пикселях"
type: docs
url: /ru/net/aspose.cells/comment/width/
---
## Comment.Width property

Представляет ширину комментария в пикселях.

```csharp
public int Width { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentPropertyWidthDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить комментарий к ячейке A1
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            
            // Установить свойства комментария
            comment.Note = "This is a sample comment";
            comment.Width = 200; // Setting the width of the comment box
            comment.Height = 50;
            
            // Сохраните книгу
            workbook.Save("CommentWidthDemo.xlsx");
        }
    }
}
```

### См. также

* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


