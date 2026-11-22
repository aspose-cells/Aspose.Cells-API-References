---
title: "Comment.HeightCM"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Comment. تمثل ارتفاع التعليق بوحدة السنتيمترات"
type: docs
url: /ar/net/aspose.cells/comment/heightcm/
---
## Comment.HeightCM property

يمثل ارتفاع التعليق، بوحدة السنتيمتر.

```csharp
public double HeightCM { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentPropertyHeightCMDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة تعليق إلى الخلية A1
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            
            // ضبط نص التعليق
            comment.Note = "Sample comment";
            
            // تعيين ارتفاع التعليق بالسنتيمترات
            comment.HeightCM = 1.5;
            
            // احفظ المصنف
            workbook.Save("CommentHeightCMDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


