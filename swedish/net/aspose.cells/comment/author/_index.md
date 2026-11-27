---
title: "Comment.Author"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Comment-egenskap. Hämtar och anger namn på den ursprungliga kommentarförfattaren"
type: docs
url: /sv/net/aspose.cells/comment/author/
---
## Comment.Author property

Hämtar och anger namn på den ursprungliga kommentarsförfattaren

```csharp
public string Author { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentPropertyAuthorDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en kommentar till cell A1
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            
            // Ställ in kommentarförfattaren och anteckningen
            comment.Author = "Carl.Yang";
            comment.Note = "This is a sample comment";

            // Visa kommentarförfattaren
            Console.WriteLine("Comment Author: " + comment.Author);
        }
    }
}
```

### Se även

* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


