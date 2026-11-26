---
title: "ThreadedCommentAuthorCollection.IndexOf"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método ThreadedCommentAuthorCollection. Obtiene el índice del objeto ThreadedCommentAuthor"
type: docs
url: /es/net/aspose.cells/threadedcommentauthorcollection/indexof/
---
## ThreadedCommentAuthorCollection.IndexOf method

Obtiene el índice del objeto ThreadedCommentAuthor

```csharp
public int IndexOf(ThreadedCommentAuthor author)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| autor | ThreadedCommentAuthor | El objeto ThreadedCommentAuthor |

### Valor de retorno

El índice en la colección ThreadedCommentAuthor

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ThreadedCommentAuthorCollectionMethodIndexOfWithThreadedCommentAuthorDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Obtenga la colección de autores de comentarios en hilo
            ThreadedCommentAuthorCollection authors = workbook.Worksheets.ThreadedCommentAuthors;

            // Agregue autores a la colección
            int johnIndex = authors.Add("John Doe", "john.doe", "provider1");
            int janeIndex = authors.Add("Jane Smith", "jane.smith", "provider2");

            // Obtenga los objetos de autor
            ThreadedCommentAuthor johnAuthor = authors[johnIndex];
            ThreadedCommentAuthor janeAuthor = authors[janeIndex];

            try
            {
                // Llame al método IndexOf para encontrar la posición de Jane Smith
                int foundIndex = authors.IndexOf(janeAuthor);
                
                // Mostrar el resultado
                Console.WriteLine($"Author '{janeAuthor.Name}' found at index: {foundIndex}");

                // Verifique que el resultado coincida con el índice esperado
                if (foundIndex == janeIndex)
                {
                    Console.WriteLine("IndexOf result matches the expected index");
                }
                else
                {
                    Console.WriteLine("IndexOf result does not match the expected index");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing IndexOf method: {ex.Message}");
            }
            
            // Guarda el libro de trabajo
            workbook.Save("ThreadedCommentAuthorIndexOfDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ThreadedCommentAuthor](../../threadedcommentauthor/)
* class [ThreadedCommentAuthorCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


