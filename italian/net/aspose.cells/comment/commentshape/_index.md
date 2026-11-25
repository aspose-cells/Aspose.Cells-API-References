---
title: "Comment.CommentShape"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Comment. Ottieni un oggetto Shape che rappresenta la forma allegata al commento specificato"
type: docs
url: /it/net/aspose.cells/comment/commentshape/
---
## Comment.CommentShape property

Ottieni un oggetto Shape che rappresenta la forma allegata al commento specificato.

```csharp
public CommentShape CommentShape { get; }
```

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un commento alla cella A1
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment1 = worksheet.Comments[commentIndex];
            comment1.Note = "This is a sample comment";

            // Ottieni il CommentShape e modifica le sue proprietà
            Shape shape = comment1.CommentShape;
            shape.Width = 200;
            shape.Height = 100;
            shape.FillFormat.ForeColor = System.Drawing.Color.LightYellow;
            shape.LineFormat.ForeColor = System.Drawing.Color.Blue;

            // Visualizza le dimensioni della forma
            Console.WriteLine("Comment shape width: " + shape.Width);
            Console.WriteLine("Comment shape height: " + shape.Height);
        }
    }
}
```

### Vedi anche

* class [CommentShape](../../../aspose.cells.drawing/commentshape/)
* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


