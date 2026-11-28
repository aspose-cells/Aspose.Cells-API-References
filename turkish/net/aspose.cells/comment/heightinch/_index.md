---
title: "Comment.HeightInch"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Comment özelliği. Yorumun yüksekliğini inç biriminde temsil eder."
type: docs
url: /tr/net/aspose.cells/comment/heightinch/
---
## Comment.HeightInch property

Yorumun yüksekliğini inç biriminde temsil eder.

```csharp
public double HeightInch { get; set; }
```

### Örnekler

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

### Ayrıca Bakınız

* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


