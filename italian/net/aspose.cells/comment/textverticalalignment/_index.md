---
title: "Comment.TextVerticalAlignment"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Comment. Ottiene e imposta il tipo di allineamento verticale del testo del commento"
type: docs
url: /it/net/aspose.cells/comment/textverticalalignment/
---
## Comment.TextVerticalAlignment property

Ottiene e imposta il tipo di allineamento verticale del testo del commento.

```csharp
public TextAlignmentType TextVerticalAlignment { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentPropertyTextVerticalAlignmentDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            int commentIndex = worksheet.Comments.Add("B3");
            Comment comment = worksheet.Comments[commentIndex];
            comment.Note = "Sample comment text";

            // Imposta l'allineamento verticale su Fill
            comment.TextVerticalAlignment = TextAlignmentType.Fill;
            Console.WriteLine("Vertical Alignment: " + comment.TextVerticalAlignment);

            // Cambia l'allineamento verticale in Center se era Fill
            if (comment.TextVerticalAlignment == TextAlignmentType.Fill)
            {
                comment.TextVerticalAlignment = TextAlignmentType.Center;
                Console.WriteLine("Changed Vertical Alignment to: " + comment.TextVerticalAlignment);
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


