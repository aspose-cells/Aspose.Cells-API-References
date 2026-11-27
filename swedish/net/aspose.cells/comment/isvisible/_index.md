---
title: "Comment.IsVisible"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Comment property. Anger om kommentaren är synlig eller inte"
type: docs
url: /sv/net/aspose.cells/comment/isvisible/
---
## Comment.IsVisible property

Representerar om kommentaren är synlig eller inte.

```csharp
public bool IsVisible { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentPropertyIsVisibleDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en kommentar till cell A1
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            comment.Note = "This is a test comment";

            // Ställ in kommentaren så att den är synlig
            comment.IsVisible = true;

            // Kontrollera om kommentaren är synlig
            if (comment.IsVisible)
            {
                Console.WriteLine("The comment is visible");
            }

            // Spara arbetsboken
            workbook.Save("CommentVisibilityDemo.xlsx");
        }
    }
}
```

### Se även

* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


