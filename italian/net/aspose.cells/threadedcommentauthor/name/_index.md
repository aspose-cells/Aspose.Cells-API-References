---
title: "ThreadedCommentAuthor.Name"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ThreadedCommentAuthor. Ottiene e imposta il nome"
type: docs
url: /it/net/aspose.cells/threadedcommentauthor/name/
---
## ThreadedCommentAuthor.Name property

Ottiene e imposta il nome.

```csharp
public string Name { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ThreadedCommentAuthorPropertyNameDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un commento e commenti in thread
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            comment.Note = "Initial comment";
            ThreadedCommentCollection threadedComments = comment.ThreadedComments;
            
            // Aggiungi commenti in thread con autori diversi
            ThreadedCommentAuthorCollection authors = workbook.Worksheets.ThreadedCommentAuthors;
            int author1Index = authors.Add("User1", "user1@example.com", "ID1");
            int author2Index = authors.Add("User2", "user2@example.com", "ID2");

            // Aggiungi commenti a thread
            threadedComments.Add("Reply from User1", authors[author1Index]);
            threadedComments.Add("Reply from User2", authors[author2Index]);

            // Dimostra l'uso della proprietà Name
            Console.WriteLine("First author name: " + threadedComments[0].Author.Name);
            Console.WriteLine("Second author name: " + threadedComments[1].Author.Name);

            // Modifica l'autore del secondo commento
            threadedComments[1].Author = authors[author1Index];
            Console.WriteLine("Updated second author name: " + threadedComments[1].Author.Name);

            // Salva la cartella di lavoro
            workbook.Save("ThreadedCommentAuthorsDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ThreadedCommentAuthor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


