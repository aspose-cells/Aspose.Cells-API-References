---
title: "Comment.WidthInch"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Comment. تمثل عرض التعليق بوحدة البوصة"
type: docs
url: /ar/net/aspose.cells/comment/widthinch/
---
## Comment.WidthInch property

يمثل عرض التعليق، بوحدة الإنش.

```csharp
public double WidthInch { get; set; }
```

### أمثلة

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

### انظر أيضًا

* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


