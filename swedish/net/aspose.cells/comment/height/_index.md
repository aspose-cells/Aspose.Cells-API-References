---
title: "Comment.Height"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Comment-egenskap. Representerar kommentaren höjd i enheten pixlar"
type: docs
url: /sv/net/aspose.cells/comment/height/
---
## Comment.Height property

Representerar kommentarsens höjd i pixlar.

```csharp
public int Height { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentPropertyHeightDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            comment.Note = "Sample comment";
            
            // Demonstrera Height-egenskapen
            comment.Height = 100;
            
            Console.WriteLine("Comment height set to: " + comment.Height);
        }
    }
}
```

### Se även

* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


