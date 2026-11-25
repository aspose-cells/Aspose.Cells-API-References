---
title: "WorksheetCollection.ThreadedCommentAuthors"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "WorksheetCollection proprietà. Restituisce l'elenco degli autori dei commenti in thread"
type: docs
url: /it/net/aspose.cells/worksheetcollection/threadedcommentauthors/
---
## WorksheetCollection.ThreadedCommentAuthors property

Ottiene l'elenco degli autori dei commenti in thread.

```csharp
public ThreadedCommentAuthorCollection ThreadedCommentAuthors { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionPropertyThreadedCommentAuthorsDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un autore di commento in thread
            int authorIndex = workbook.Worksheets.ThreadedCommentAuthors.Add("Demo Author", "demo", "DA");

            // Ottieni l'autore che abbiamo appena aggiunto
            ThreadedCommentAuthor author = workbook.Worksheets.ThreadedCommentAuthors[authorIndex];

            // Aggiungi commenti in thread alla cella C2
            AddThreadedComment(worksheet, "C2", "First comment", author);
            AddThreadedComment(worksheet, "C2", "Second comment", author);
            AddThreadedComment(worksheet, "C2", "Third comment", author);

            // Salva la cartella di lavoro
            workbook.Save("ThreadedCommentsDemo.xlsx");
        }

        private static void AddThreadedComment(Worksheet worksheet, string cellName, string text, ThreadedCommentAuthor author)
        {
            // Ottieni la cella dove vogliamo aggiungere il commento
            Cell cell = worksheet.Cells[cellName];
            
            // Aggiungi un commento in thread (restituisce void, non ThreadedComment)
            worksheet.Comments.AddThreadedComment(cellName, text, author);
        }
    }
}
```

### Vedi anche

* class [ThreadedCommentAuthorCollection](../../threadedcommentauthorcollection/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


