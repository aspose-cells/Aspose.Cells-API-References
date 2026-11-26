---
title: "ThreadedComment.Author"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ThreadedComment. Obtiene el autor del comentario"
type: docs
url: /es/net/aspose.cells/threadedcomment/author/
---
## ThreadedComment.Author property

Obtiene el autor del comentario.

```csharp
public ThreadedCommentAuthor Author { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ThreadedCommentPropertyAuthorDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Obtener el autor predeterminado del comentario en hilo del libro de trabajo
                ThreadedCommentAuthor author = workbook.Worksheets.ThreadedCommentAuthors[0];
                author.Name = "John Doe";
                author.UserId = "john.doe@example.com";

                // Agregar un comentario en hilo a la celda A1 (fila 0, columna 0)
                worksheet.Comments.AddThreadedComment(0, 0, "Sample comment", author);

                // Obtener el primer comentario en hilo
                ThreadedComment comment = worksheet.Comments[0].ThreadedComments[0];

                // Mostrar el valor de la propiedad Author (operación de lectura)
                Console.WriteLine("Author Name: " + comment.Author.Name);
                Console.WriteLine("Author UserId: " + comment.Author.UserId);
                Console.WriteLine("Author ProviderId: " + comment.Author.ProviderId);

                // Demostrar la configuración de la propiedad Author (ya que es de lectura/escritura)
                ThreadedCommentAuthor newAuthor = workbook.Worksheets.ThreadedCommentAuthors[0];
                newAuthor.Name = "Jane Smith";
                newAuthor.UserId = "jane.smith@example.com";
                comment.Author = newAuthor;

                // Mostrar el valor actualizado de la propiedad Author
                Console.WriteLine("Updated Author Name: " + comment.Author.Name);
                Console.WriteLine("Updated Author UserId: " + comment.Author.UserId);

                // Guarda el libro de trabajo
                workbook.Save("ThreadedCommentAuthorDemo.xlsx");
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

* class [ThreadedCommentAuthor](../../threadedcommentauthor/)
* class [ThreadedComment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


