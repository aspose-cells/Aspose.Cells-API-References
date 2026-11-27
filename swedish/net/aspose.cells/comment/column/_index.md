---
title: "Comment.Column"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Comment property. Hämtar kolumnindexet för kommentaren"
type: docs
url: /sv/net/aspose.cells/comment/column/
---
## Comment.Column property

Hämtar kolumnindexet för kommentaren.

```csharp
public int Column { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentPropertyColumnDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en kommentar i cell B5 (kolumnindex 1)
            int commentRow = 4;
            int commentColumn = 1;
            Comment comment = worksheet.Comments[worksheet.Comments.Add(commentRow, commentColumn)];

            // Ställ in kommentartext
            comment.Note = "This is a sample comment";

            // Demonstrera användning av Column-egenskapen
            Console.WriteLine("Comment is in column: " + comment.Column);

            // Verifiera att kolumnindexet matchar där vi placerade den
            if (comment.Column == commentColumn)
            {
                Console.WriteLine("Column property correctly returns the comment's column index");
            }
        }
    }
}
```

### Se även

* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


