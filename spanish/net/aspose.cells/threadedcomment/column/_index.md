---
title: "ThreadedComment.Column"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ThreadedComment. Obtiene el índice de columna del comentario"
type: docs
url: /es/net/aspose.cells/threadedcomment/column/
---
## ThreadedComment.Column property

Obtiene el índice de columna del comentario.

```csharp
public int Column { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ThreadedCommentPropertyColumnDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            try
            {
                // Cree primero un autor de comentario en hilo
                ThreadedCommentAuthor author = workbook.Worksheets.ThreadedCommentAuthors[0];
                
                // Agregar un comentario en hilo a la celda A1 (fila 0, columna 0)
                int commentRow = 0;
                int commentColumn = 0;
                worksheet.Comments.AddThreadedComment(commentRow, commentColumn, "Sample comment text", author);
                
                // Obtener el primer comentario en hilo
                ThreadedComment comment = worksheet.Comments[0].ThreadedComments[0];
                
                // Muestre el valor de la propiedad Column (solo lectura)
                Console.WriteLine("Threaded comment column index: " + comment.Column);
                
                // Verifique que el índice de columna coincida con el lugar donde colocamos el comentario
                if (comment.Column == commentColumn)
                {
                    Console.WriteLine("Comment is correctly placed in column " + commentColumn);
                }
                
                // Guarda el libro de trabajo
                workbook.Save("ThreadedCommentColumnDemo.xlsx");
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


