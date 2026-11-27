---
title: "Comment.Width"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Comment property. Representerar bredden på kommentaren i enheten pixlar"
type: docs
url: /sv/net/aspose.cells/comment/width/
---
## Comment.Width property

Representerar bredden på kommentaren, i enhet pixlar.

```csharp
public int Width { get; set; }
```

### Exempel

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

            // Lägg till en kommentar till cell A1
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            
            // Ställ in kommentarens egenskaper
            comment.Note = "This is a sample comment";
            comment.Width = 200; // Setting the width of the comment box
            comment.Height = 50;
            
            // Spara arbetsboken
            workbook.Save("CommentWidthDemo.xlsx");
        }
    }
}
```

### Se även

* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


