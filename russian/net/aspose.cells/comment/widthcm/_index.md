---
title: "Comment.WidthCM"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Comment. Представляет ширину комментария в сантиметрах"
type: docs
url: /ru/net/aspose.cells/comment/widthcm/
---
## Comment.WidthCM property

Представляет ширину комментария в сантиметрах.

```csharp
public double WidthCM { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentPropertyWidthCMDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            comment.Note = "Sample comment";
            comment.WidthCM = 5.0;

            Console.WriteLine($"Comment width set to: {comment.WidthCM} cm");
        }
    }
}
```

### См. также

* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


