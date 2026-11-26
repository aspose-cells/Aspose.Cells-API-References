---
title: "ThreadedComment.Row"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ThreadedComment. Obtiene el índice de fila del comentario"
type: docs
url: /es/net/aspose.cells/threadedcomment/row/
---
## ThreadedComment.Row property

Obtiene el índice de fila del comentario.

```csharp
public int Row { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ThreadedCommentPropertyRowDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            try
            {
                // Crear un autor de comentario en hilo
                ThreadedCommentAuthor author = workbook.Worksheets.ThreadedCommentAuthors[0];
                author.Name = "Test Author";
                author.UserId = "test@example.com";
                
                // Agregar un comentario en hilo a la celda B2 (fila 1, columna 1)
                worksheet.Comments.AddThreadedComment(1, 1, "Sample threaded comment", author);
                
                // Obtener el primer comentario en hilo
                ThreadedComment comment = worksheet.Comments[0].ThreadedComments[0];
                
                // Mostrar el valor de la propiedad Row (solo lectura)
                Console.WriteLine("Threaded comment row index: " + comment.Row);
                
                // Verificar que el índice de fila coincida con el lugar donde se colocó el comentario
                if (comment.Row == 1)
                {
                    Console.WriteLine("Comment is correctly placed in row 1");
                }
                
                // Guarda el libro de trabajo
                workbook.Save("ThreadedCommentRowDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [ThreadedComment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


