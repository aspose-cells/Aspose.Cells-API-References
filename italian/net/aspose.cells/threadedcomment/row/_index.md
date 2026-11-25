---
title: "ThreadedComment.Row"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ThreadedComment. Ottiene l'indice di riga del commento"
type: docs
url: /it/net/aspose.cells/threadedcomment/row/
---
## ThreadedComment.Row property

Ottiene l'indice di riga del commento.

```csharp
public int Row { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ThreadedCommentPropertyRowDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            try
            {
                // Crea un autore di commenti a thread
                ThreadedCommentAuthor author = workbook.Worksheets.ThreadedCommentAuthors[0];
                author.Name = "Test Author";
                author.UserId = "test@example.com";
                
                // Aggiungi un commento a thread alla cella B2 (riga 1, colonna 1)
                worksheet.Comments.AddThreadedComment(1, 1, "Sample threaded comment", author);
                
                // Ottieni il primo commento a thread
                ThreadedComment comment = worksheet.Comments[0].ThreadedComments[0];
                
                // Visualizza il valore della proprietà Row (sola lettura)
                Console.WriteLine("Threaded comment row index: " + comment.Row);
                
                // Verifica che l'indice di riga corrisponda a dove abbiamo posizionato il commento
                if (comment.Row == 1)
                {
                    Console.WriteLine("Comment is correctly placed in row 1");
                }
                
                // Salva la cartella di lavoro
                workbook.Save("ThreadedCommentRowDemo.xlsx");
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


