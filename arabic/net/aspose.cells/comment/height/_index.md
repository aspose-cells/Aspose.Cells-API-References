---
title: "Comment.Height"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Comment. تمثل ارتفاع التعليق بوحدة البكسل"
type: docs
url: /ar/net/aspose.cells/comment/height/
---
## Comment.Height property

يمثل ارتفاع التعليق، بوحدة البكسل.

```csharp
public int Height { get; set; }
```

### أمثلة

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
            
            // عرض خاصية Height
            comment.Height = 100;
            
            Console.WriteLine("Comment height set to: " + comment.Height);
        }
    }
}
```

### انظر أيضًا

* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


