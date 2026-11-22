---
title: "MsoLineFormat.Weight"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية MsoLineFormat. تُرجع أو تُعيّن وزن الخط بوحدات النقاط (pt)"
type: docs
url: /ar/net/aspose.cells.drawing/msolineformat/weight/
---
## MsoLineFormat.Weight property

إرجاع أو تعيين وزن الخط، بوحدات النقاط.

```csharp
public double Weight { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class MsoLineFormatPropertyWeightDemo
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
            
            // تعيين نص التعليق
            comment.Note = "Sample comment";
            
            // الوصول إلى تنسيق خط شكل التعليق وتعيين الوزن
            comment.CommentShape.LineFormat.Weight = 0.75;
            
            // احفظ المصنف
            workbook.Save("output.xlsx");
            
            // تحقق من أن الوزن تم تعيينه بشكل صحيح
            Console.WriteLine("Line weight: " + worksheet.Comments[0].CommentShape.LineFormat.Weight);
        }
    }
}
```

### انظر أيضًا

* class [MsoLineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


