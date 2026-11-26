---
title: "ThreadedComment.Notes"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ThreadedComment. Obtiene y establece el texto del comentario"
type: docs
url: /es/net/aspose.cells/threadedcomment/notes/
---
## ThreadedComment.Notes property

Obtiene y establece el texto del comentario.

```csharp
public string Notes { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ThreadedCommentPropertyNotesDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo y obtener la primera hoja de cálculo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Crear u obtener un autor de comentario en hilo
                ThreadedCommentAuthor author = workbook.Worksheets.ThreadedCommentAuthors["User1"];
                author.Name = "User1";

                // Agregar un comentario en hilo a la celda A1 (fila 0, columna 0) con texto inicial
                worksheet.Comments.AddThreadedComment(0, 0, "Initial comment text", author);

                // Recuperar el comentario en hilo recién añadido
                ThreadedComment threadedComment = worksheet.Comments[0].ThreadedComments[0];

                // Actualizar la propiedad Notes (el texto del comentario)
                threadedComment.Notes = "Updated comment notes";

                // Leer y mostrar el valor de la propiedad Notes
                Console.WriteLine("Threaded comment Notes: " + threadedComment.Notes);

                // Guardar el libro de trabajo (opcional)
                workbook.Save("ThreadedCommentNotesDemo.xlsx");
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


