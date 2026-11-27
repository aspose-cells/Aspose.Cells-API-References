---
title: "Comment.HeightInch"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Comment-egenskap. Representerar kommentarsens höjd i tum"
type: docs
url: /sv/net/aspose.cells/comment/heightinch/
---
## Comment.HeightInch property

Representerar kommentarsens höjd i tum.

```csharp
public double HeightInch { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentPropertyHeightInchDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            
            comment.HeightInch = 1.5;
            Console.WriteLine("Comment height set to: " + comment.HeightInch + " inches");
        }
    }
}
```

### Se även

* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


