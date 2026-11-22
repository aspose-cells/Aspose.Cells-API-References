---
title: "Comment.Font"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Comment. تحصل على خط التعليق"
type: docs
url: /ar/net/aspose.cells/comment/font/
---
## Comment.Font property

يحصل على خط التعليق.

```csharp
public Font Font { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentPropertyFontDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة تعليق إلى الخلية A1
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            comment.Note = "Sample comment";

            // الوصول إلى خصائص الخط للتعليق وتعديلها
            Aspose.Cells.Font font = comment.Font;
            font.Size = 12;
            font.Name = "Arial";
            font.Color = System.Drawing.Color.Red;
            font.IsBold = true;

            // احفظ المصنف
            workbook.Save("CommentFontDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Font](../../font/)
* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


