---
title: "Comment.Width"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Comment-Eigenschaft. Gibt die Breite des Kommentars in Pixeln an"
type: docs
url: /de/net/aspose.cells/comment/width/
---
## Comment.Width property

Stellt die Breite des Kommentars in Pixeln dar.

```csharp
public int Width { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentPropertyWidthDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Einen Kommentar zur Zelle A1 hinzufügen
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            
            // Setze Kommentar‑Eigenschaften
            comment.Note = "This is a sample comment";
            comment.Width = 200; // Setting the width of the comment box
            comment.Height = 50;
            
            // Speichere die Arbeitsmappe
            workbook.Save("CommentWidthDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


