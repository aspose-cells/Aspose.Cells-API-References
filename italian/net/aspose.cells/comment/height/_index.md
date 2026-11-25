---
title: "Comment.Height"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Comment. Rappresenta l'altezza del commento in unità di pixel"
type: docs
url: /it/net/aspose.cells/comment/height/
---
## Comment.Height property

Rappresenta l'Altezza del commento, in unità di pixel.

```csharp
public int Height { get; set; }
```

### Esempi

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
            
            // Dimostra la proprietà Height
            comment.Height = 100;
            
            Console.WriteLine("Comment height set to: " + comment.Height);
        }
    }
}
```

### Vedi anche

* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


