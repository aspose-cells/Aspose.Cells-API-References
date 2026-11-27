---
title: "Comment.Row"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Comment-egenskap. Hämtar radindexet för kommentaren"
type: docs
url: /sv/net/aspose.cells/comment/row/
---
## Comment.Row property

Hämtar radindexet för kommentaren.

```csharp
public int Row { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentPropertyRowDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en kommentar till cell A1
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment1 = worksheet.Comments[commentIndex];
            comment1.Note = "This is a sample comment";

            // Hämta och visa radindexet för den kommenterade cellen
            int row = comment1.Row;
            Console.WriteLine("The comment is in row: " + row);

            // Lägg till en annan kommentar till cell B3
            commentIndex = worksheet.Comments.Add("B3");
            Comment comment2 = worksheet.Comments[commentIndex];
            comment2.Note = "Another comment";

            // Visa radindex för den andra kommentaren
            Console.WriteLine("Second comment is in row: " + comment2.Row);
        }
    }
}
```

### Se även

* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


