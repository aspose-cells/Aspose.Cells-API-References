---
title: "Comment.Height"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Comment özelliği. Yorumun piksel birimindeki yüksekliğini temsil eder"
type: docs
url: /tr/net/aspose.cells/comment/height/
---
## Comment.Height property

Yorumun yüksekliğini piksel biriminde temsil eder.

```csharp
public int Height { get; set; }
```

### Örnekler

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
            
            // Height özelliğini göster
            comment.Height = 100;
            
            Console.WriteLine("Comment height set to: " + comment.Height);
        }
    }
}
```

### Ayrıca Bakınız

* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


