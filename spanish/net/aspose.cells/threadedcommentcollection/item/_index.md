---
title: "ThreadedCommentCollection.Item"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ThreadedCommentCollection. Obtiene el comentario en hilo por el índice específico"
type: docs
url: /es/net/aspose.cells/threadedcommentcollection/item/
---
## ThreadedCommentCollection indexer

Obtiene el comentario en hilo por el índice específico.

```csharp
public ThreadedComment this[int index] { get; }
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
    public class ThreadedCommentCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un comentario
            Comment comment = worksheet.Comments[worksheet.Comments.Add("A1")];
            comment.Note = "Initial comment";

            // Agregar comentarios en hilo
            ThreadedCommentCollection threadedComments = comment.ThreadedComments;
            ThreadedCommentAuthorCollection authors = workbook.Worksheets.ThreadedCommentAuthors;
            
            // Agregar autores
            int author1Index = authors.Add("User1", "user1@example.com", "ID1");
            int author2Index = authors.Add("User2", "user2@example.com", "ID2");

            // Agregar comentarios en hilo
            threadedComments.Add("Reply 1", authors[author1Index]);
            threadedComments.Add("Reply 2", authors[author2Index]);

            // Demostrar el uso de la propiedad Item
            ThreadedComment firstComment = threadedComments[0];
            ThreadedComment secondComment = threadedComments[1];

            Console.WriteLine("First comment author: " + firstComment.Author.Name);
            Console.WriteLine("Second comment author: " + secondComment.Author.Name);

            // Modificar el autor del segundo comentario
            secondComment.Author = authors[author1Index];
            Console.WriteLine("Updated second comment author: " + secondComment.Author.Name);

            // Guarda el libro de trabajo
            workbook.Save("ThreadedCommentsDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ThreadedComment](../../threadedcomment/)
* class [ThreadedCommentCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


