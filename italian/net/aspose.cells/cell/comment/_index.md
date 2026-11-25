---
title: "Cell.Comment"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Cell. Ottiene il commento di questa cella"
type: docs
url: /it/net/aspose.cells/cell/comment/
---
## Cell.Comment property

Restituisce il commento di questa cella.

```csharp
public Comment Comment { get; }
```

### Osservazioni

Se non esiste alcun commento applicato alla cella, restituisce null.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellPropertyCommentDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un commento alla cella A1
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Sample Cell");

            // Aggiungi un commento alla cella
            Comment comment = cell.Comment;
            if (comment == null)
            {
                // Crea un nuovo commento se non esiste
                int commentIndex = worksheet.Comments.Add("A1");
                comment = worksheet.Comments[commentIndex];
                comment.Author = "Author Name";
                comment.Note = "This is a sample comment";
            }

            try
            {
                // Visualizza le proprietà del commento
                Console.WriteLine("Comment Author: " + comment.Author);
                Console.WriteLine("Comment Note: " + comment.Note);
                Console.WriteLine("Comment Row: " + comment.Row);
                Console.WriteLine("Comment Column: " + comment.Column);
                Console.WriteLine("Comment is Visible: " + comment.IsVisible);

                // Modifica alcune proprietà del commento
                comment.Note = "Updated comment text";
                comment.IsVisible = true;

                // Visualizza la nota del commento aggiornata
                Console.WriteLine("Updated Comment Note: " + comment.Note);

                // Salva la cartella di lavoro
                workbook.Save("CommentDemo.xlsx");
                Console.WriteLine("Comment has been demonstrated and saved to CommentDemo.xlsx");
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

* class [Comment](../../comment/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


