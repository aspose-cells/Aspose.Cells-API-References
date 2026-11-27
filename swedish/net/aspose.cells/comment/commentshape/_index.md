---
title: "Comment.CommentShape"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Comment property. Hämta ett Shape-objekt som representerar formen som är bifogad till den angivna kommentaren"
type: docs
url: /sv/net/aspose.cells/comment/commentshape/
---
## Comment.CommentShape property

Hämta ett Shape-objekt som representerar formen som är bifogad till den angivna kommentaren.

```csharp
public CommentShape CommentShape { get; }
```

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en kommentar till cell A1
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment1 = worksheet.Comments[commentIndex];
            comment1.Note = "This is a sample comment";

            // Hämta CommentShape och ändra dess egenskaper
            Shape shape = comment1.CommentShape;
            shape.Width = 200;
            shape.Height = 100;
            shape.FillFormat.ForeColor = System.Drawing.Color.LightYellow;
            shape.LineFormat.ForeColor = System.Drawing.Color.Blue;

            // Visa formens dimensioner
            Console.WriteLine("Comment shape width: " + shape.Width);
            Console.WriteLine("Comment shape height: " + shape.Height);
        }
    }
}
```

### Se även

* class [CommentShape](../../../aspose.cells.drawing/commentshape/)
* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


