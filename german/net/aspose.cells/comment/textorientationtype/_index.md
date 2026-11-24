---
title: "Comment.TextOrientationType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Comment-Eigenschaft. Liest und setzt den Textorientierungstyp des Kommentars"
type: docs
url: /de/net/aspose.cells/comment/textorientationtype/
---
## Comment.TextOrientationType property

Liest und setzt den Orientierungstyp des Textes im Kommentar.

```csharp
public TextOrientationType TextOrientationType { get; set; }
```

### Beispiele

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

            // Einen Kommentar zur Zelle A1 hinzufügen
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            comment.Note = "Sample comment text";

            // Setzen Sie die Anfangsorientierung auf NoRotation
            comment.TextOrientationType = TextOrientationType.NoRotation;
            Console.WriteLine("Initial orientation: " + comment.TextOrientationType);

            // Ändern Sie die Orientierung zu TopToBottom, wenn sie derzeit NoRotation ist
            if (comment.TextOrientationType == TextOrientationType.NoRotation)
            {
                comment.TextOrientationType = TextOrientationType.TopToBottom;
                Console.WriteLine("Changed orientation to: " + comment.TextOrientationType);
            }

            // Speichere die Arbeitsmappe
            workbook.Save("CommentOrientationDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [TextOrientationType](../../textorientationtype/)
* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


