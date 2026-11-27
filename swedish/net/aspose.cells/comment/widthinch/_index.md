---
title: "Comment.WidthInch"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Comment-egenskap. Representerar kommentarsens bredd i tum"
type: docs
url: /sv/net/aspose.cells/comment/widthinch/
---
## Comment.WidthInch property

Representerar bredden på kommentaren, i enhet tum.

```csharp
public double WidthInch { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentPropertyWidthInchDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            comment.Note = "Sample comment";
            
            comment.WidthInch = 1.5;
            
            Console.WriteLine("Comment width set to: " + comment.WidthInch + " inches");
        }
    }
}
```

### Se även

* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


