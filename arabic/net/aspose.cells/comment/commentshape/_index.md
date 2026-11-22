---
title: "Comment.CommentShape"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Comment. احصل على كائن Shape الذي يمثل الشكل المرتبط بالتعليق المحدد"
type: docs
url: /ar/net/aspose.cells/comment/commentshape/
---
## Comment.CommentShape property

احصل على كائن Shape الذي يمثل الشكل المرفق بالتعليق المحدد.

```csharp
public CommentShape CommentShape { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class CommentPropertyCommentShapeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة تعليق إلى الخلية A1
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment1 = worksheet.Comments[commentIndex];
            comment1.Note = "This is a sample comment";

            // احصل على CommentShape وعدل خصائصه
            Shape shape = comment1.CommentShape;
            shape.Width = 200;
            shape.Height = 100;
            shape.FillFormat.ForeColor = System.Drawing.Color.LightYellow;
            shape.LineFormat.ForeColor = System.Drawing.Color.Blue;

            // عرض أبعاد الشكل
            Console.WriteLine("Comment shape width: " + shape.Width);
            Console.WriteLine("Comment shape height: " + shape.Height);
        }
    }
}
```

### انظر أيضًا

* class [CommentShape](../../../aspose.cells.drawing/commentshape/)
* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


