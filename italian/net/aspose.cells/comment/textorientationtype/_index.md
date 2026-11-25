---
title: "Comment.TextOrientationType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Comment. Ottiene e imposta il tipo di orientamento del testo del commento"
type: docs
url: /it/net/aspose.cells/comment/textorientationtype/
---
## Comment.TextOrientationType property

Ottiene e imposta il tipo di orientamento del testo del commento.

```csharp
public TextOrientationType TextOrientationType { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentPropertyTextOrientationTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un commento alla cella A1
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            comment.Note = "Sample comment text";

            // Imposta l'orientamento iniziale su NoRotation
            comment.TextOrientationType = TextOrientationType.NoRotation;
            Console.WriteLine("Initial orientation: " + comment.TextOrientationType);

            // Cambia l'orientamento in TopToBottom se attualmente è NoRotation
            if (comment.TextOrientationType == TextOrientationType.NoRotation)
            {
                comment.TextOrientationType = TextOrientationType.TopToBottom;
                Console.WriteLine("Changed orientation to: " + comment.TextOrientationType);
            }

            // Salva la cartella di lavoro
            workbook.Save("CommentOrientationDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [TextOrientationType](../../textorientationtype/)
* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


