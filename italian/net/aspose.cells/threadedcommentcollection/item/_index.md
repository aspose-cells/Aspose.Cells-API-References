---
title: "ThreadedCommentCollection.Item"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ThreadedCommentCollection. Ottiene il commento a thread tramite l'indice specifico"
type: docs
url: /it/net/aspose.cells/threadedcommentcollection/item/
---
## ThreadedCommentCollection indexer

Ottiene il commento a thread per l'indice specifico.

```csharp
public ThreadedComment this[int index] { get; }
```

| Parametro | Descrizione |
| --- | --- |
| indice | L'indice |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ThreadedCommentCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un commento
            Comment comment = worksheet.Comments[worksheet.Comments.Add("A1")];
            comment.Note = "Initial comment";

            // Aggiungi commenti a thread
            ThreadedCommentCollection threadedComments = comment.ThreadedComments;
            ThreadedCommentAuthorCollection authors = workbook.Worksheets.ThreadedCommentAuthors;
            
            // Aggiungi autori
            int author1Index = authors.Add("User1", "user1@example.com", "ID1");
            int author2Index = authors.Add("User2", "user2@example.com", "ID2");

            // Aggiungi commenti a thread
            threadedComments.Add("Reply 1", authors[author1Index]);
            threadedComments.Add("Reply 2", authors[author2Index]);

            // Dimostra l'uso della proprietà Item
            ThreadedComment firstComment = threadedComments[0];
            ThreadedComment secondComment = threadedComments[1];

            Console.WriteLine("First comment author: " + firstComment.Author.Name);
            Console.WriteLine("Second comment author: " + secondComment.Author.Name);

            // Modifica l'autore del secondo commento
            secondComment.Author = authors[author1Index];
            Console.WriteLine("Updated second comment author: " + secondComment.Author.Name);

            // Salva la cartella di lavoro
            workbook.Save("ThreadedCommentsDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ThreadedComment](../../threadedcomment/)
* class [ThreadedCommentCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


