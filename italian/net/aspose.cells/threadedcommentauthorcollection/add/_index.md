---
title: "ThreadedCommentAuthorCollection.Add"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo ThreadedCommentAuthorCollection. Aggiunge una persona di commento a thread"
type: docs
url: /it/net/aspose.cells/threadedcommentauthorcollection/add/
---
## ThreadedCommentAuthorCollection.Add method

Aggiunge una persona al commento in thread.

```csharp
public int Add(string name, string userId, string providerId)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| name | String | Il nome della persona. |
| userId | String |  |
| providerId | String | L'ID del provider |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ThreadedCommentAuthorCollectionMethodAddWithStringStringStringDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un autore di commento in thread
            int authorIndex = workbook.Worksheets.ThreadedCommentAuthors.Add("Test Author", "testuser", "TA");

            // Ottieni l'autore aggiunto
            ThreadedCommentAuthor author = workbook.Worksheets.ThreadedCommentAuthors[authorIndex];

            // Aggiungi commenti a thread usando l'autore
            worksheet.Comments.AddThreadedComment("C2", "First comment", author);
            worksheet.Comments.AddThreadedComment("C2", "Second comment", author);

            // Salva la cartella di lavoro
            workbook.Save("ThreadedCommentsExample.xlsx");
        }
    }
}
```

### Vedi anche

* class [ThreadedCommentAuthorCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


