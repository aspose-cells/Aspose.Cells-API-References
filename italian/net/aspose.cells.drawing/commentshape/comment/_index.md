---
title: "CommentShape.Comment"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà CommentShape. Ottiene l'oggetto commento"
type: docs
url: /it/net/aspose.cells.drawing/commentshape/comment/
---
## CommentShape.Comment property

Ottiene l'oggetto commento.

```csharp
public Comment Comment { get; }
```

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un commento alla cella A1
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            comment.Note = "This is a sample comment";
            
            // Ottieni la forma del commento e dimostra la proprietà Comment
            CommentShape commentShape = worksheet.Comments[commentIndex].CommentShape;
            Comment retrievedComment = commentShape.Comment;
            
            // Visualizza il testo del commento
            Console.WriteLine("Comment Text: " + retrievedComment.Note);
        }
    }
}
```

### Vedi anche

* class [Comment](../../../aspose.cells/comment/)
* class [CommentShape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


