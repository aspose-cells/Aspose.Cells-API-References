---
title: "ThreadedComment.Column"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ThreadedComment. Ottiene l'indice di colonna del commento"
type: docs
url: /it/net/aspose.cells/threadedcomment/column/
---
## ThreadedComment.Column property

Ottiene l'indice di colonna del commento.

```csharp
public int Column { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ThreadedCommentPropertyColumnDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            try
            {
                // Crea prima un autore di commento a thread
                ThreadedCommentAuthor author = workbook.Worksheets.ThreadedCommentAuthors[0];
                
                // Aggiungi un commento a thread alla cella A1 (riga 0, colonna 0)
                int commentRow = 0;
                int commentColumn = 0;
                worksheet.Comments.AddThreadedComment(commentRow, commentColumn, "Sample comment text", author);
                
                // Ottieni il primo commento a thread
                ThreadedComment comment = worksheet.Comments[0].ThreadedComments[0];
                
                // Visualizza il valore della proprietà Column (sola lettura)
                Console.WriteLine("Threaded comment column index: " + comment.Column);
                
                // Verifica che l'indice di colonna corrisponda a dove abbiamo posizionato il commento
                if (comment.Column == commentColumn)
                {
                    Console.WriteLine("Comment is correctly placed in column " + commentColumn);
                }
                
                // Salva la cartella di lavoro
                workbook.Save("ThreadedCommentColumnDemo.xlsx");
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


