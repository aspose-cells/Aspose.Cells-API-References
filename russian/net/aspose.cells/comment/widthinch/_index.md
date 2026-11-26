---
title: "Comment.WidthInch"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Comment. Представляет ширину комментария в дюймах"
type: docs
url: /ru/net/aspose.cells/comment/widthinch/
---
## Comment.WidthInch property

Представляет ширину комментария в дюймах.

```csharp
public double WidthInch { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentPropertyWidthInchDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            comment.Note = "Sample comment";
            
            comment.WidthInch = 1.5;
            
            Console.WriteLine("Comment width set to: " + comment.WidthInch + " inches");
        }
    }
}
```

### См. также

* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


