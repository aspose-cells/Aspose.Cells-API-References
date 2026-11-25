---
title: "Comment.Column"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Comment. Ottiene l'indice di colonna del commento"
type: docs
url: /it/net/aspose.cells/comment/column/
---
## Comment.Column property

Ottiene l'indice di colonna del commento.

```csharp
public int Column { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentPropertyColumnDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un commento alla cella B5 (indice colonna 1)
            int commentRow = 4;
            int commentColumn = 1;
            Comment comment = worksheet.Comments[worksheet.Comments.Add(commentRow, commentColumn)];

            // Imposta il testo del commento
            comment.Note = "This is a sample comment";

            // Dimostra l'uso della proprietà Column
            Console.WriteLine("Comment is in column: " + comment.Column);

            // Verifica che l'indice di colonna corrisponda a dove lo abbiamo posizionato
            if (comment.Column == commentColumn)
            {
                Console.WriteLine("Column property correctly returns the comment's column index");
            }
        }
    }
}
```

### Vedi anche

* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


