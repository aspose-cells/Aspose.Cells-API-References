---
title: "ThreadedCommentAuthorCollection.Item"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ThreadedCommentAuthorCollection. Obtiene la persona que crea los comentarios en hilo"
type: docs
url: /es/net/aspose.cells/threadedcommentauthorcollection/item/
---
## ThreadedCommentAuthorCollection indexer (1 of 2)

Obtiene la persona que crea los comentarios en hilo.

```csharp
public ThreadedCommentAuthor this[int index] { get; }
```

| Parámetro | Descripción |
| --- | --- |
| índice | El índice |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ThreadedCommentAuthorCollectionPropertyItemDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            ThreadedCommentAuthorCollection authors = workbook.Worksheets.ThreadedCommentAuthors;
            
            // Agregue autores y demuestre el uso de la propiedad Item
            authors.Add("John Doe", "john.doe@example.com", "JD");
            authors.Add("Jane Smith", "jane.smith@example.com", "JS");
            
            // Acceda al autor usando la propiedad Item
            ThreadedCommentAuthor firstAuthor = authors[0];
            Console.WriteLine($"First author: {firstAuthor.Name}, {firstAuthor.UserId}");
            
            // Establezca la persona actual usando la propiedad Item
            authors.CurrentPerson = authors[1];
            Console.WriteLine($"Current person: {authors.CurrentPerson.Name}");

            // Agregar comentarios en hilo
            CommentCollection comments = workbook.Worksheets[0].Comments;
            comments.AddThreadedComment("A1", "Comment from " + authors[0].Name, authors[0]);
            comments.AddThreadedComment("A1", "Reply from " + authors[1].Name, authors[1]);

            workbook.Save("ThreadedCommentAuthorsDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ThreadedCommentAuthor](../../threadedcommentauthor/)
* class [ThreadedCommentAuthorCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ThreadedCommentAuthorCollection indexer (2 of 2)

Obtiene la persona que crea los comentarios en hilo.

```csharp
public ThreadedCommentAuthor this[string name] { get; }
```

| Parámetro | Descripción |
| --- | --- |
| name | El nombre del autor. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ThreadedCommentAuthorCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            try
            {
                // Acceder a la ThreadedCommentAuthorCollection
                ThreadedCommentAuthorCollection authors = workbook.Worksheets.ThreadedCommentAuthors;

                // Agregue algunos autores para demostrar la propiedad Item
                authors.Add("John Doe", "john.doe@example.com", "JD");
                authors.Add("Jane Smith", "jane.smith@example.com", "JS");

                // Acceda a los autores usando la propiedad Item (indexador)
                ThreadedCommentAuthor firstAuthor = authors[0];
                ThreadedCommentAuthor secondAuthor = authors[1];

                // Muestre la información del autor obtenida a través de la propiedad Item
                Console.WriteLine($"First author: {firstAuthor.Name}, {firstAuthor.UserId}");
                Console.WriteLine($"Second author: {secondAuthor.Name}, {secondAuthor.UserId}");

                // Establezca la persona actual usando uno de los autores accedidos mediante la propiedad Item
                authors.CurrentPerson = authors[0];
                Console.WriteLine($"Current person set to: {authors.CurrentPerson.Name}");

                // Guarda el libro de trabajo
                workbook.Save("ThreadedCommentAuthorsItemDemo.xlsx");
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
* class [ThreadedCommentAuthorCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


