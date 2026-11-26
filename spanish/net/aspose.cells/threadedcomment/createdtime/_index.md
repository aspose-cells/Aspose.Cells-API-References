---
title: "ThreadedComment.CreatedTime"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ThreadedComment. Obtiene y establece la hora de creación de este comentario en hilo"
type: docs
url: /es/net/aspose.cells/threadedcomment/createdtime/
---
## ThreadedComment.CreatedTime property

Obtiene y establece la hora de creación de este comentario en hilo.

```csharp
public DateTime CreatedTime { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ThreadedCommentPropertyCreatedTimeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crear un autor de comentario en hilo
            ThreadedCommentAuthor author = workbook.Worksheets.ThreadedCommentAuthors["User1"];
            
            // Agregar un comentario a la celda A1
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            
            // Agregar un comentario en hilo
            int threadedCommentIndex = comment.ThreadedComments.Add("Test comment", author);
            ThreadedComment threadedComment = comment.ThreadedComments[threadedCommentIndex];
            
            // Demostrar la propiedad CreatedTime
            Console.WriteLine("Threaded comment created at: " + threadedComment.CreatedTime);
            
            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [ThreadedComment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


