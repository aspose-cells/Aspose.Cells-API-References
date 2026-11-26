---
title: "ThreadedCommentAuthor.UserId"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ThreadedCommentAuthor. Obtiene y establece el id del usuario"
type: docs
url: /es/net/aspose.cells/threadedcommentauthor/userid/
---
## ThreadedCommentAuthor.UserId property

Obtiene y establece el id del usuario.

```csharp
public string UserId { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ThreadedCommentAuthorPropertyUserIdDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Agregar un autor de comentario en hilo con nombre, userId y providerId
                int authorIndex = workbook.Worksheets.ThreadedCommentAuthors.Add("John Doe", "JD123", "PROVIDER123");

                // Obtener el objeto ThreadedCommentAuthor
                ThreadedCommentAuthor author = workbook.Worksheets.ThreadedCommentAuthors[authorIndex];

                // Mostrar el valor de UserId (operación de lectura)
                Console.WriteLine("Author UserId: " + author.UserId);

                // Demostrar la configuración de un nuevo UserId (operación de escritura)
                author.UserId = "NEW_USER_ID";
                Console.WriteLine("Updated UserId: " + author.UserId);

                // Crear un comentario en hilo usando el autor
                worksheet.Comments.AddThreadedComment("A1", "This is a sample comment", author);

                // Guarda el libro de trabajo
                workbook.Save("UserIdDemo.xlsx");

                Console.WriteLine("UserId property demonstration completed successfully.");
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

* class [ThreadedCommentAuthor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


