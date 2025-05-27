---
title: Comment.HeightInch
second_title: Aspose.Cells for .NET API Reference
description: Comment property. Represents the height of the comment in unit of inches
type: docs
url: /net/aspose.cells/comment/heightinch/
---
## Comment.HeightInch property

Represents the height of the comment, in unit of inches.

```csharp
public double HeightInch { get; set; }
```

### Examples

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

### See Also

* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


