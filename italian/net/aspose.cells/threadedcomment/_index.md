---
title: "Classe ThreadedComment"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.ThreadedComment. Rappresenta il commento a thread"
type: docs
url: /it/net/aspose.cells/threadedcomment/
---
## ThreadedComment class

Rappresenta il commento in thread.

```csharp
public class ThreadedComment
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Author](../../aspose.cells/threadedcomment/author/) { get; set; } | Ottiene l'autore del commento. |
| [Column](../../aspose.cells/threadedcomment/column/) { get; } | Ottiene l'indice di colonna del commento. |
| [CreatedTime](../../aspose.cells/threadedcomment/createdtime/) { get; set; } | Ottiene e imposta l'ora di creazione di questo commento a thread. |
| [Notes](../../aspose.cells/threadedcomment/notes/) { get; set; } | Ottiene e imposta il testo del commento. |
| [Row](../../aspose.cells/threadedcomment/row/) { get; } | Ottiene l'indice di riga del commento. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassThreadedCommentDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi autori alla cartella di lavoro
            int author1Id = workbook.Worksheets.ThreadedCommentAuthors.Add("User1", "user1@example.com", "1");
            int author2Id = workbook.Worksheets.ThreadedCommentAuthors.Add("User2", "", "2");
            
            // Ottieni riferimenti all'autore
            ThreadedCommentAuthor author1 = workbook.Worksheets.ThreadedCommentAuthors[author1Id];
            ThreadedCommentAuthor author2 = workbook.Worksheets.ThreadedCommentAuthors[author2Id];
            
            // Aggiungi un commento alla cella A1
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            
            // Aggiungi commento a thread al commento
            int threadedCommentIndex = comment.ThreadedComments.Add("This is a threaded comment", author1);
            ThreadedComment threadedComment = comment.ThreadedComments[threadedCommentIndex];
            
            // Imposta proprietà aggiuntive
            threadedComment.Notes = "Additional notes";
            
            // Aggiungi una risposta al commento a thread
            int replyIndex = comment.ThreadedComments.Add("This is a reply", author2);
            ThreadedComment reply = comment.ThreadedComments[replyIndex];
            
            // Salva la cartella di lavoro
            workbook.Save("ThreadedCommentDemo.xlsx");
            
            Console.WriteLine("Threaded comment demo completed.");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


