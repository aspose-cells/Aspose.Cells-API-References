---
title: "Comment.Font"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Comment-egenskap. Hämtar kommentaren teckensnitt"
type: docs
url: /sv/net/aspose.cells/comment/font/
---
## Comment.Font property

Hämtar kommentarsfonten.

```csharp
public Font Font { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentPropertyFontDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en kommentar till cell A1
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            comment.Note = "Sample comment";

            // Åtkomst till och ändra teckensnittsegenskaperna för kommentaren
            Aspose.Cells.Font font = comment.Font;
            font.Size = 12;
            font.Name = "Arial";
            font.Color = System.Drawing.Color.Red;
            font.IsBold = true;

            // Spara arbetsboken
            workbook.Save("CommentFontDemo.xlsx");
        }
    }
}
```

### Se även

* class [Font](../../font/)
* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


