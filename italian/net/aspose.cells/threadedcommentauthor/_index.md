---
title: "Classe ThreadedCommentAuthor"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.ThreadedCommentAuthor. Rappresenta la persona che crea i commenti a thread."
type: docs
url: /it/net/aspose.cells/threadedcommentauthor/
---
## ThreadedCommentAuthor class

Rappresenta la persona che crea i commenti in thread.

```csharp
public class ThreadedCommentAuthor
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Name](../../aspose.cells/threadedcommentauthor/name/) { get; set; } | Ottiene e imposta il nome. |
| [ProviderId](../../aspose.cells/threadedcommentauthor/providerid/) { get; set; } | Ottiene l'ID del provider. |
| [UserId](../../aspose.cells/threadedcommentauthor/userid/) { get; set; } | Ottiene e imposta l'ID dell'utente. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassThreadedCommentAuthorDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un commento
            int commentIndex = worksheet.Comments.Add("C1");
            Comment comment = worksheet.Comments[commentIndex];
            comment.Note = "Initial comment";
            
            // Aggiungi gli autori dei commenti in thread
            int authorIndex1 = workbook.Worksheets.ThreadedCommentAuthors.Add("Author1", "user1", "");
            ThreadedCommentAuthor author1 = workbook.Worksheets.ThreadedCommentAuthors[authorIndex1];
            
            // Aggiungi un commento in thread
            int threadedCommentIndex = comment.ThreadedComments.Add("Threaded comment text", author1);
            ThreadedComment threadedComment = comment.ThreadedComments[threadedCommentIndex];
            
            // Accedi e modifica l'autore
            Console.WriteLine("Original author: " + threadedComment.Author.Name);
            threadedComment.Author.Name = "ModifiedAuthor";
            Console.WriteLine("Modified author: " + threadedComment.Author.Name);

            // Crea un nuovo autore e assegnalo
            int authorIndex2 = workbook.Worksheets.ThreadedCommentAuthors.Add("Author2", "user2", "");
            ThreadedCommentAuthor author2 = workbook.Worksheets.ThreadedCommentAuthors[authorIndex2];
            threadedComment.Author = author2;
            Console.WriteLine("New author: " + threadedComment.Author.Name);
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


