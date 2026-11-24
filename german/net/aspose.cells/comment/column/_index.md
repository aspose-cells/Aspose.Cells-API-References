---
title: "Comment.Column"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Comment-Eigenschaft. Gibt den Spaltenindex des Kommentars zurück"
type: docs
url: /de/net/aspose.cells/comment/column/
---
## Comment.Column property

Liefert den Spaltenindex des Kommentars.

```csharp
public int Column { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentPropertyColumnDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge einen Kommentar zu Zelle B5 hinzu (Spaltenindex 1)
            int commentRow = 4;
            int commentColumn = 1;
            Comment comment = worksheet.Comments[worksheet.Comments.Add(commentRow, commentColumn)];

            // Setze Kommentartext
            comment.Note = "This is a sample comment";

            // Demonstration der Verwendung der Column-Eigenschaft
            Console.WriteLine("Comment is in column: " + comment.Column);

            // Überprüfe, ob der Spaltenindex mit der Position übereinstimmt, an der wir ihn platziert haben
            if (comment.Column == commentColumn)
            {
                Console.WriteLine("Column property correctly returns the comment's column index");
            }
        }
    }
}
```

### Siehe auch

* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


