---
title: "ThreadedCommentAuthor.Name"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ThreadedCommentAuthor. Obtiene y establece el nombre"
type: docs
url: /es/net/aspose.cells/threadedcommentauthor/name/
---
## ThreadedCommentAuthor.Name property

Obtiene y establece el nombre.

```csharp
public string Name { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ThreadedCommentAuthorPropertyNameDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un comentario y comentarios en hilo
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            comment.Note = "Initial comment";
            ThreadedCommentCollection threadedComments = comment.ThreadedComments;
            
            // Agregar comentarios en hilo con diferentes autores
            ThreadedCommentAuthorCollection authors = workbook.Worksheets.ThreadedCommentAuthors;
            int author1Index = authors.Add("User1", "user1@example.com", "ID1");
            int author2Index = authors.Add("User2", "user2@example.com", "ID2");

            // Agregar comentarios en hilo
            threadedComments.Add("Reply from User1", authors[author1Index]);
            threadedComments.Add("Reply from User2", authors[author2Index]);

            // Demostrar el uso de la propiedad Name
            Console.WriteLine("First author name: " + threadedComments[0].Author.Name);
            Console.WriteLine("Second author name: " + threadedComments[1].Author.Name);

            // Cambiar el autor del segundo comentario
            threadedComments[1].Author = authors[author1Index];
            Console.WriteLine("Updated second author name: " + threadedComments[1].Author.Name);

            // Guarda el libro de trabajo
            workbook.Save("ThreadedCommentAuthorsDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ThreadedCommentAuthor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


