---
title: "Comment.TextHorizontalAlignment"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Comment-Eigenschaft. Liest und setzt den horizontalen Ausrichtungstyp des Textes im Kommentar"
type: docs
url: /de/net/aspose.cells/comment/texthorizontalalignment/
---
## Comment.TextHorizontalAlignment property

Liest und setzt den horizontalen Ausrichtungstyp des Textes im Kommentar.

```csharp
public TextAlignmentType TextHorizontalAlignment { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentPropertyTextHorizontalAlignmentDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Einen Kommentar zur Zelle A1 hinzufügen
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            comment.Note = "Sample comment text";

            // Setzen Sie die anfängliche horizontale Ausrichtung auf Fill
            comment.TextHorizontalAlignment = TextAlignmentType.Fill;
            Console.WriteLine("Initial alignment: " + comment.TextHorizontalAlignment);

            // Ändern Sie die Ausrichtung zu Center, wenn sie Fill war
            if (comment.TextHorizontalAlignment == TextAlignmentType.Fill)
            {
                comment.TextHorizontalAlignment = TextAlignmentType.Center;
                Console.WriteLine("Updated alignment: " + comment.TextHorizontalAlignment);
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


