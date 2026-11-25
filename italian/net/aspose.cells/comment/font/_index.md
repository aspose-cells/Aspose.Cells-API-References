---
title: "Comment.Font"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Comment. Ottiene il font del commento"
type: docs
url: /it/net/aspose.cells/comment/font/
---
## Comment.Font property

Ottiene il carattere del commento.

```csharp
public Font Font { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentPropertyFontDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un commento alla cella A1
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            comment.Note = "Sample comment";

            // Accedi e modifica le proprietà del font del commento
            Aspose.Cells.Font font = comment.Font;
            font.Size = 12;
            font.Name = "Arial";
            font.Color = System.Drawing.Color.Red;
            font.IsBold = true;

            // Salva la cartella di lavoro
            workbook.Save("CommentFontDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Font](../../font/)
* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


