---
title: "Comment.TextHorizontalAlignment"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Comment‑egenskap. Hämtar och anger den horisontella justeringstypen för kommentaren"
type: docs
url: /sv/net/aspose.cells/comment/texthorizontalalignment/
---
## Comment.TextHorizontalAlignment property

Hämtar och anger den horisontella justeringstypen för kommentaren.

```csharp
public TextAlignmentType TextHorizontalAlignment { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentPropertyTextHorizontalAlignmentDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en kommentar till cell A1
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            comment.Note = "Sample comment text";

            // Ställ in initial horisontell justering till Fill
            comment.TextHorizontalAlignment = TextAlignmentType.Fill;
            Console.WriteLine("Initial alignment: " + comment.TextHorizontalAlignment);

            // Ändra justeringen till Center om den var Fill
            if (comment.TextHorizontalAlignment == TextAlignmentType.Fill)
            {
                comment.TextHorizontalAlignment = TextAlignmentType.Center;
                Console.WriteLine("Updated alignment: " + comment.TextHorizontalAlignment);
            }
        }
    }
}
```

### Se även

* enum [TextAlignmentType](../../textalignmenttype/)
* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


