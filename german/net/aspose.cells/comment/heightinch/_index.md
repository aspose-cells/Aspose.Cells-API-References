---
title: "Comment.HeightInch"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Comment-Eigenschaft. Gibt die Höhe des Kommentars in Zoll an"
type: docs
url: /de/net/aspose.cells/comment/heightinch/
---
## Comment.HeightInch property

Stellt die Höhe des Kommentars in Zoll dar.

```csharp
public double HeightInch { get; set; }
```

### Beispiele

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

### Siehe auch

* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


