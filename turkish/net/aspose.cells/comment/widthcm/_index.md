---
title: "Comment.WidthCM"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Comment özelliği. Yorumun genişliğini santimetre biriminde temsil eder."
type: docs
url: /tr/net/aspose.cells/comment/widthcm/
---
## Comment.WidthCM property

Yorumun genişliğini santimetre biriminde temsil eder.

```csharp
public double WidthCM { get; set; }
```

### Örnekler

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

### Ayrıca Bakınız

* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


