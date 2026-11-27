---
title: "Comment.WidthCM"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Comment-egenskap. Representerar kommentarsens bredd i centimeter"
type: docs
url: /sv/net/aspose.cells/comment/widthcm/
---
## Comment.WidthCM property

Representerar bredden på kommentaren, i enhet centimeter.

```csharp
public double WidthCM { get; set; }
```

### Exempel

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

### Se även

* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


