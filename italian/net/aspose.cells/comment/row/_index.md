---
title: "Comment.Row"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Comment. Ottiene l'indice di riga del commento"
type: docs
url: /it/net/aspose.cells/comment/row/
---
## Comment.Row property

Ottiene l'indice di riga del commento.

```csharp
public int Row { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentPropertyRowDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un commento alla cella A1
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment1 = worksheet.Comments[commentIndex];
            comment1.Note = "This is a sample comment";

            // Ottieni e visualizza l'indice di riga della cella commentata
            int row = comment1.Row;
            Console.WriteLine("The comment is in row: " + row);

            // Aggiungi un altro commento alla cella B3
            commentIndex = worksheet.Comments.Add("B3");
            Comment comment2 = worksheet.Comments[commentIndex];
            comment2.Note = "Another comment";

            // Visualizza l'indice di riga del secondo commento
            Console.WriteLine("Second comment is in row: " + comment2.Row);
        }
    }
}
```

### Vedi anche

* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


