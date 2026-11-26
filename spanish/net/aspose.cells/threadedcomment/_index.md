---
title: "Clase ThreadedComment"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.ThreadedComment. Representa el comentario en hilo"
type: docs
url: /es/net/aspose.cells/threadedcomment/
---
## ThreadedComment class

Representa el comentario en hilo.

```csharp
public class ThreadedComment
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Author](../../aspose.cells/threadedcomment/author/) { get; set; } | Obtiene el autor del comentario. |
| [Column](../../aspose.cells/threadedcomment/column/) { get; } | Obtiene el índice de columna del comentario. |
| [CreatedTime](../../aspose.cells/threadedcomment/createdtime/) { get; set; } | Obtiene y establece la hora de creación de este comentario en hilo. |
| [Notes](../../aspose.cells/threadedcomment/notes/) { get; set; } | Obtiene y establece el texto del comentario. |
| [Row](../../aspose.cells/threadedcomment/row/) { get; } | Obtiene el índice de fila del comentario. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassThreadedCommentDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar autores al libro de trabajo
            int author1Id = workbook.Worksheets.ThreadedCommentAuthors.Add("User1", "user1@example.com", "1");
            int author2Id = workbook.Worksheets.ThreadedCommentAuthors.Add("User2", "", "2");
            
            // Obtener referencias de autor
            ThreadedCommentAuthor author1 = workbook.Worksheets.ThreadedCommentAuthors[author1Id];
            ThreadedCommentAuthor author2 = workbook.Worksheets.ThreadedCommentAuthors[author2Id];
            
            // Agregar un comentario a la celda A1
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            
            // Agregar comentario en hilo al comentario
            int threadedCommentIndex = comment.ThreadedComments.Add("This is a threaded comment", author1);
            ThreadedComment threadedComment = comment.ThreadedComments[threadedCommentIndex];
            
            // Establecer propiedades adicionales
            threadedComment.Notes = "Additional notes";
            
            // Agregar una respuesta al comentario en hilo
            int replyIndex = comment.ThreadedComments.Add("This is a reply", author2);
            ThreadedComment reply = comment.ThreadedComments[replyIndex];
            
            // Guarda el libro de trabajo
            workbook.Save("ThreadedCommentDemo.xlsx");
            
            Console.WriteLine("Threaded comment demo completed.");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


