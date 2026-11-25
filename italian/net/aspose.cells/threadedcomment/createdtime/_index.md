---
title: "ThreadedComment.CreatedTime"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ThreadedComment. Ottiene e imposta l'ora di creazione di questo commento a thread"
type: docs
url: /it/net/aspose.cells/threadedcomment/createdtime/
---
## ThreadedComment.CreatedTime property

Ottiene e imposta l'ora di creazione di questo commento a thread.

```csharp
public DateTime CreatedTime { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ThreadedCommentPropertyCreatedTimeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crea un autore di commenti a thread
            ThreadedCommentAuthor author = workbook.Worksheets.ThreadedCommentAuthors["User1"];
            
            // Aggiungi un commento alla cella A1
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            
            // Aggiungi un commento in thread
            int threadedCommentIndex = comment.ThreadedComments.Add("Test comment", author);
            ThreadedComment threadedComment = comment.ThreadedComments[threadedCommentIndex];
            
            // Dimostra la proprietà CreatedTime
            Console.WriteLine("Threaded comment created at: " + threadedComment.CreatedTime);
            
            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [ThreadedComment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


