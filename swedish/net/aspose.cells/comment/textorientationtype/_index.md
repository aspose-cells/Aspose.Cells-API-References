---
title: "Comment.TextOrientationType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Comment‑egenskap. Hämtar och anger textorienteringstypen för kommentaren"
type: docs
url: /sv/net/aspose.cells/comment/textorientationtype/
---
## Comment.TextOrientationType property

Hämtar och anger textorienteringstypen för kommentaren.

```csharp
public TextOrientationType TextOrientationType { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentPropertyTextOrientationTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en kommentar till cell A1
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            comment.Note = "Sample comment text";

            // Ställ in initial orientering till NoRotation
            comment.TextOrientationType = TextOrientationType.NoRotation;
            Console.WriteLine("Initial orientation: " + comment.TextOrientationType);

            // Ändra orientering till TopToBottom om den för närvarande är NoRotation
            if (comment.TextOrientationType == TextOrientationType.NoRotation)
            {
                comment.TextOrientationType = TextOrientationType.TopToBottom;
                Console.WriteLine("Changed orientation to: " + comment.TextOrientationType);
            }

            // Spara arbetsboken
            workbook.Save("CommentOrientationDemo.xlsx");
        }
    }
}
```

### Se även

* enum [TextOrientationType](../../textorientationtype/)
* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


