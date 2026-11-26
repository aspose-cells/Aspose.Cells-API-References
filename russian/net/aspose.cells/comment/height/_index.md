---
title: "Comment.Height"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Comment. Представляет высоту комментария в пикселях"
type: docs
url: /ru/net/aspose.cells/comment/height/
---
## Comment.Height property

Представляет высоту комментария в пикселях.

```csharp
public int Height { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentPropertyHeightDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            comment.Note = "Sample comment";
            
            // Продемонстрировать свойство Height
            comment.Height = 100;
            
            Console.WriteLine("Comment height set to: " + comment.Height);
        }
    }
}
```

### См. также

* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


