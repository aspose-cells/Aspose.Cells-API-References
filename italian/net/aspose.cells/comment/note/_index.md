---
title: "Comment.Note"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Comment. Rappresenta il contenuto del commento"
type: docs
url: /it/net/aspose.cells/comment/note/
---
## Comment.Note property

Rappresenta il contenuto del commento.

```csharp
public string Note { get; set; }
```

### Osservazioni

Se questo è un commento a thread, la nota non può essere modificata, altrimenti MS Excel non potrebbe elaborarlo come commento a thread.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentPropertyNoteDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un commento alla cella A1
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment1 = worksheet.Comments[commentIndex];
            
            // Imposta la nota per il commento
            comment1.Note = "First note.";
            
            // Verifica che la nota sia stata impostata
            Console.WriteLine("Comment note: " + comment1.Note);
        }
    }
}
```

### Vedi anche

* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


