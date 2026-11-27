---
title: "CommentShape.Comment"
second_title: "Aspose.Cells för .NET API‑referens"
description: "CommentShape‑egenskap. Hämtar kommentarsobjektet"
type: docs
url: /sv/net/aspose.cells.drawing/commentshape/comment/
---
## CommentShape.Comment property

Hämtar kommentarsobjektet.

```csharp
public Comment Comment { get; }
```

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en kommentar till cell A1
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            comment.Note = "This is a sample comment";
            
            // Hämta kommentarsformen och demonstrera Comment‑egenskapen
            CommentShape commentShape = worksheet.Comments[commentIndex].CommentShape;
            Comment retrievedComment = commentShape.Comment;
            
            // Visa kommentartexten
            Console.WriteLine("Comment Text: " + retrievedComment.Note);
        }
    }
}
```

### Se även

* class [Comment](../../../aspose.cells/comment/)
* class [CommentShape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


