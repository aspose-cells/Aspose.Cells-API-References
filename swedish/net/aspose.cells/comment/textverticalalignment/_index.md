---
title: "Comment.TextVerticalAlignment"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Comment‑egenskap. Hämtar och anger den vertikala justeringstypen för kommentaren"
type: docs
url: /sv/net/aspose.cells/comment/textverticalalignment/
---
## Comment.TextVerticalAlignment property

Hämtar och anger den vertikala justeringstypen för kommentaren.

```csharp
public TextAlignmentType TextVerticalAlignment { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentPropertyTextVerticalAlignmentDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            int commentIndex = worksheet.Comments.Add("B3");
            Comment comment = worksheet.Comments[commentIndex];
            comment.Note = "Sample comment text";

            // Ställ in vertikal justering till Fill
            comment.TextVerticalAlignment = TextAlignmentType.Fill;
            Console.WriteLine("Vertical Alignment: " + comment.TextVerticalAlignment);

            // Ändra vertikal justering till Center om den var Fill
            if (comment.TextVerticalAlignment == TextAlignmentType.Fill)
            {
                comment.TextVerticalAlignment = TextAlignmentType.Center;
                Console.WriteLine("Changed Vertical Alignment to: " + comment.TextVerticalAlignment);
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


