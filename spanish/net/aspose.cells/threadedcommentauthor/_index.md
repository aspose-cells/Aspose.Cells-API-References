---
title: "Clase ThreadedCommentAuthor"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.ThreadedCommentAuthor. Representa a la persona que crea los comentarios en hilo"
type: docs
url: /es/net/aspose.cells/threadedcommentauthor/
---
## ThreadedCommentAuthor class

Representa a la persona que crea los comentarios en hilo.

```csharp
public class ThreadedCommentAuthor
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Name](../../aspose.cells/threadedcommentauthor/name/) { get; set; } | Obtiene y establece el nombre. |
| [ProviderId](../../aspose.cells/threadedcommentauthor/providerid/) { get; set; } | Obtiene el id del proveedor. |
| [UserId](../../aspose.cells/threadedcommentauthor/userid/) { get; set; } | Obtiene y establece el id del usuario. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassThreadedCommentAuthorDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un comentario
            int commentIndex = worksheet.Comments.Add("C1");
            Comment comment = worksheet.Comments[commentIndex];
            comment.Note = "Initial comment";
            
            // Agregar autores de comentarios en hilo
            int authorIndex1 = workbook.Worksheets.ThreadedCommentAuthors.Add("Author1", "user1", "");
            ThreadedCommentAuthor author1 = workbook.Worksheets.ThreadedCommentAuthors[authorIndex1];
            
            // Agregar un comentario en hilo
            int threadedCommentIndex = comment.ThreadedComments.Add("Threaded comment text", author1);
            ThreadedComment threadedComment = comment.ThreadedComments[threadedCommentIndex];
            
            // Acceder y modificar el autor
            Console.WriteLine("Original author: " + threadedComment.Author.Name);
            threadedComment.Author.Name = "ModifiedAuthor";
            Console.WriteLine("Modified author: " + threadedComment.Author.Name);

            // Crear un nuevo autor y asignarlo
            int authorIndex2 = workbook.Worksheets.ThreadedCommentAuthors.Add("Author2", "user2", "");
            ThreadedCommentAuthor author2 = workbook.Worksheets.ThreadedCommentAuthors[authorIndex2];
            threadedComment.Author = author2;
            Console.WriteLine("New author: " + threadedComment.Author.Name);
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


