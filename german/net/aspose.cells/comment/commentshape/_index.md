---
title: "Comment.CommentShape"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Comment-Eigenschaft. Gibt ein Shape-Objekt zurück, das die dem angegebenen Kommentar zugefügte Form darstellt"
type: docs
url: /de/net/aspose.cells/comment/commentshape/
---
## Comment.CommentShape property

Erhalte ein Shape-Objekt, das die dem angegebenen Kommentar zugefügte Form darstellt.

```csharp
public CommentShape CommentShape { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class CommentPropertyCommentShapeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Einen Kommentar zur Zelle A1 hinzufügen
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment1 = worksheet.Comments[commentIndex];
            comment1.Note = "This is a sample comment";

            // Hole das CommentShape und ändere seine Eigenschaften
            Shape shape = comment1.CommentShape;
            shape.Width = 200;
            shape.Height = 100;
            shape.FillFormat.ForeColor = System.Drawing.Color.LightYellow;
            shape.LineFormat.ForeColor = System.Drawing.Color.Blue;

            // Zeige die Formabmessungen an
            Console.WriteLine("Comment shape width: " + shape.Width);
            Console.WriteLine("Comment shape height: " + shape.Height);
        }
    }
}
```

### Siehe auch

* class [CommentShape](../../../aspose.cells.drawing/commentshape/)
* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


