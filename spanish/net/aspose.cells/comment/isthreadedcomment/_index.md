---
title: "Comment.IsThreadedComment"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Comment. Indica si este comentario es un comentario con hilos"
type: docs
url: /es/net/aspose.cells/comment/isthreadedcomment/
---
## Comment.IsThreadedComment property

Indica si este comentario es un comentario en hilo.

```csharp
public bool IsThreadedComment { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentPropertyIsThreadedCommentDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un comentario regular
            Comment regularComment = worksheet.Comments[worksheet.Comments.Add("A1")];
            regularComment.Note = "This is a regular comment";
            regularComment.Author = "User1";

            // Agregar un comentario con hilos (asumiendo que la API soporta agregar comentarios con hilos)
            Comment threadedComment = worksheet.Comments[worksheet.Comments.Add("B1")];
            threadedComment.Note = "This is a threaded comment";
            threadedComment.Author = "User2";

            // Verificar tipos de comentario
            Console.WriteLine("Comment at A1 is threaded: " + regularComment.IsThreadedComment);
            Console.WriteLine("Comment at B1 is threaded: " + threadedComment.IsThreadedComment);

            // Procesar comentarios según su tipo
            foreach (Comment comment in worksheet.Comments)
            {
                if (comment.IsThreadedComment)
                {
                    Console.WriteLine($"Threaded comment found at {CellsHelper.CellIndexToName(comment.Row, comment.Column)}");
                    Console.WriteLine($"Author: {comment.Author}, Note: {comment.Note}");
                }
                else
                {
                    Console.WriteLine($"Regular comment found at {CellsHelper.CellIndexToName(comment.Row, comment.Column)}");
                }
            }
        }
    }
}
```

### Ver también

* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


