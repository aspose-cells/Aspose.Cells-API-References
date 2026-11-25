---
title: "ThreadedComment.Notes"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ThreadedComment. Ottiene e imposta il testo del commento"
type: docs
url: /it/net/aspose.cells/threadedcomment/notes/
---
## ThreadedComment.Notes property

Ottiene e imposta il testo del commento.

```csharp
public string Notes { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ThreadedCommentPropertyNotesDemo
    {
        public static void Run()
        {
            // Crea una nuova cartella di lavoro e ottieni il primo foglio di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Crea o ottieni un autore di commenti a thread
                ThreadedCommentAuthor author = workbook.Worksheets.ThreadedCommentAuthors["User1"];
                author.Name = "User1";

                // Aggiungi un commento a thread alla cella A1 (riga 0, colonna 0) con testo iniziale
                worksheet.Comments.AddThreadedComment(0, 0, "Initial comment text", author);

                // Recupera il commento a thread appena aggiunto
                ThreadedComment threadedComment = worksheet.Comments[0].ThreadedComments[0];

                // Aggiorna la proprietà Notes (il testo del commento)
                threadedComment.Notes = "Updated comment notes";

                // Leggi e visualizza il valore della proprietà Notes
                Console.WriteLine("Threaded comment Notes: " + threadedComment.Notes);

                // Salva la cartella di lavoro (opzionale)
                workbook.Save("ThreadedCommentNotesDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [ThreadedComment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


