---
title: "Comment.TextVerticalAlignment"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Comment-Eigenschaft. Liest und setzt den vertikalen Ausrichtungstyp des Textes im Kommentar"
type: docs
url: /de/net/aspose.cells/comment/textverticalalignment/
---
## Comment.TextVerticalAlignment property

Liest und setzt den vertikalen Ausrichtungstyp des Textes im Kommentar.

```csharp
public TextAlignmentType TextVerticalAlignment { get; set; }
```

### Beispiele

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

            // Setzen Sie die vertikale Ausrichtung auf Fill
            comment.TextVerticalAlignment = TextAlignmentType.Fill;
            Console.WriteLine("Vertical Alignment: " + comment.TextVerticalAlignment);

            // Ändern Sie die vertikale Ausrichtung zu Center, wenn sie Fill war
            if (comment.TextVerticalAlignment == TextAlignmentType.Fill)
            {
                comment.TextVerticalAlignment = TextAlignmentType.Center;
                Console.WriteLine("Changed Vertical Alignment to: " + comment.TextVerticalAlignment);
            }
        }
    }
}
```

### Siehe auch

* enum [TextAlignmentType](../../textalignmenttype/)
* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


