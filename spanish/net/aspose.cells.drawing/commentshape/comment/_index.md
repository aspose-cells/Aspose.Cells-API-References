---
title: "CommentShape.Comment"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad CommentShape. Obtiene el objeto de comentario"
type: docs
url: /es/net/aspose.cells.drawing/commentshape/comment/
---
## CommentShape.Comment property

Obtiene el objeto de comentario.

```csharp
public Comment Comment { get; }
```

### Ejemplos

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
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un comentario a la celda A1
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            comment.Note = "This is a sample comment";
            
            // Obtener la forma de comentario y demostrar la propiedad Comment
            CommentShape commentShape = worksheet.Comments[commentIndex].CommentShape;
            Comment retrievedComment = commentShape.Comment;
            
            // Mostrar el texto del comentario
            Console.WriteLine("Comment Text: " + retrievedComment.Note);
        }
    }
}
```

### Ver también

* class [Comment](../../../aspose.cells/comment/)
* class [CommentShape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


