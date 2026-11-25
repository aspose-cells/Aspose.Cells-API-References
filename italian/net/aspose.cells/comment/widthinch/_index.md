---
title: "Comment.WidthInch"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Comment. Rappresenta la larghezza del commento in unità di pollici"
type: docs
url: /it/net/aspose.cells/comment/widthinch/
---
## Comment.WidthInch property

Rappresenta la larghezza del commento, in unità di pollici.

```csharp
public double WidthInch { get; set; }
```

### Esempi

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

### Vedi anche

* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


