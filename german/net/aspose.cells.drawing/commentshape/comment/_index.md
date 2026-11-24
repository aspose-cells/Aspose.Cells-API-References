---
title: "CommentShape.Comment"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "CommentShape Eigenschaft. Gibt das Kommentarobjekt zurück"
type: docs
url: /de/net/aspose.cells.drawing/commentshape/comment/
---
## CommentShape.Comment property

Liest das Kommentarobjekt.

```csharp
public Comment Comment { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class CommentShapePropertyCommentDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Einen Kommentar zur Zelle A1 hinzufügen
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            comment.Note = "This is a sample comment";
            
            // Kommentarform abrufen und die Comment-Eigenschaft demonstrieren
            CommentShape commentShape = worksheet.Comments[commentIndex].CommentShape;
            Comment retrievedComment = commentShape.Comment;
            
            // Kommentartext anzeigen
            Console.WriteLine("Comment Text: " + retrievedComment.Note);
        }
    }
}
```

### Siehe auch

* class [Comment](../../../aspose.cells/comment/)
* class [CommentShape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


