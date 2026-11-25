---
title: "Comment.WidthCM"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Comment. Rappresenta la larghezza del commento in unità di centimetri"
type: docs
url: /it/net/aspose.cells/comment/widthcm/
---
## Comment.WidthCM property

Rappresenta la larghezza del commento, in unità di centimetri.

```csharp
public double WidthCM { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentPropertyWidthCMDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            comment.Note = "Sample comment";
            comment.WidthCM = 5.0;

            Console.WriteLine($"Comment width set to: {comment.WidthCM} cm");
        }
    }
}
```

### Vedi anche

* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


