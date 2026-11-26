---
title: "ThreadedCommentAuthor.ProviderId"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ThreadedCommentAuthor. Obtiene el id del proveedor"
type: docs
url: /es/net/aspose.cells/threadedcommentauthor/providerid/
---
## ThreadedCommentAuthor.ProviderId property

Obtiene el id del proveedor.

```csharp
public string ProviderId { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ThreadedCommentAuthorPropertyProviderIdDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            try
            {
                // Agregar un autor de comentario en hilo y obtener su índice
                int authorIndex = workbook.Worksheets.ThreadedCommentAuthors.Add("John Doe", "JD123", "PROVIDER123");
                
                // Obtener el objeto ThreadedCommentAuthor
                ThreadedCommentAuthor author = workbook.Worksheets.ThreadedCommentAuthors[authorIndex];
                
                // Mostrar el valor de ProviderId (operación de lectura)
                Console.WriteLine("Author ProviderId: " + author.ProviderId);
                
                // Crear un comentario en hilo usando el autor
                worksheet.Comments.AddThreadedComment("A1", "This is a sample comment", author);
                
                // Guarda el libro de trabajo
                workbook.Save("ThreadedCommentAuthorDemo.xlsx");
                
                Console.WriteLine("Demo completed successfully.");
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


