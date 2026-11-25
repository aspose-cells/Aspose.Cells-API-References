---
title: "Comment.TextHorizontalAlignment"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Comment. Ottiene e imposta il tipo di allineamento orizzontale del testo del commento"
type: docs
url: /it/net/aspose.cells/comment/texthorizontalalignment/
---
## Comment.TextHorizontalAlignment property

Ottiene e imposta il tipo di allineamento orizzontale del testo del commento.

```csharp
public TextAlignmentType TextHorizontalAlignment { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentPropertyTextHorizontalAlignmentDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un commento alla cella A1
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            comment.Note = "Sample comment text";

            // Imposta l'allineamento orizzontale iniziale su Fill
            comment.TextHorizontalAlignment = TextAlignmentType.Fill;
            Console.WriteLine("Initial alignment: " + comment.TextHorizontalAlignment);

            // Cambia l'allineamento in Center se era Fill
            if (comment.TextHorizontalAlignment == TextAlignmentType.Fill)
            {
                comment.TextHorizontalAlignment = TextAlignmentType.Center;
                Console.WriteLine("Updated alignment: " + comment.TextHorizontalAlignment);
            }
        }
    }
}
```

### Vedi anche

* enum [TextAlignmentType](../../textalignmenttype/)
* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


