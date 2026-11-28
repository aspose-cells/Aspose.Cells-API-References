---
title: "Comment.WidthInch"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Comment özelliği. Yorumun genişliğini inç biriminde temsil eder."
type: docs
url: /tr/net/aspose.cells/comment/widthinch/
---
## Comment.WidthInch property

Yorumun genişliğini inç biriminde temsil eder.

```csharp
public double WidthInch { get; set; }
```

### Örnekler

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

### Ayrıca Bakınız

* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


