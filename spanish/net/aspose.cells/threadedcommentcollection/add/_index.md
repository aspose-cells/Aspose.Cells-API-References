---
title: "ThreadedCommentCollection.Add"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método ThreadedCommentCollection. Añade un comentario en hilo"
type: docs
url: /es/net/aspose.cells/threadedcommentcollection/add/
---
## ThreadedCommentCollection.Add method

Agrega un comentario en hilo.

```csharp
public int Add(string text, ThreadedCommentAuthor author)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| texto | String | El texto del comentario en hilo. |
| autor | ThreadedCommentAuthor | El autor del comentario en hilo |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ThreadedCommentCollectionMethodAddWithStringThreadedCommentDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar algunos datos para contexto
            worksheet.Cells["A1"].Value = "Sample Data";

            try
            {
                // Crear un autor de comentario en hilo usando ThreadedCommentAuthorCollection
                ThreadedCommentAuthorCollection authors = workbook.Worksheets.ThreadedCommentAuthors;
                int authorIndex = authors.Add("John Doe", "john.doe@example.com", "EXAMPLE_PROVIDER");
                ThreadedCommentAuthor author = authors[authorIndex];

                // Acceder a la colección de comentarios en hilo de una celda
                Comment comment = worksheet.Comments[worksheet.Comments.Add("A1")];
                ThreadedCommentCollection threadedComments = comment.ThreadedComments;

                // Llamar al método Add con parámetros String y ThreadedCommentAuthor
                int commentIndex = threadedComments.Add("This is a threaded comment", author);

                // Mostrar el resultado
                Console.WriteLine($"Added threaded comment at index: {commentIndex}");
                Console.WriteLine($"Comment text: {threadedComments[commentIndex].Notes}");
                Console.WriteLine($"Author: {threadedComments[commentIndex].Author.Name}");

                // Guarda el libro de trabajo
                workbook.Save("ThreadedCommentAddDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
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
* class [ThreadedCommentCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


