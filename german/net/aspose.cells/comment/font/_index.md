---
title: "Comment.Font"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Comment-Eigenschaft. Gibt die Schriftart des Kommentars zurück"
type: docs
url: /de/net/aspose.cells/comment/font/
---
## Comment.Font property

Liest die Schriftart des Kommentars.

```csharp
public Font Font { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentPropertyFontDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Einen Kommentar zur Zelle A1 hinzufügen
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            comment.Note = "Sample comment";

            // Greifen Sie auf die Schriftarteigenschaften des Kommentars zu und ändern Sie sie
            Aspose.Cells.Font font = comment.Font;
            font.Size = 12;
            font.Name = "Arial";
            font.Color = System.Drawing.Color.Red;
            font.IsBold = true;

            // Speichere die Arbeitsmappe
            workbook.Save("CommentFontDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Font](../../font/)
* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


