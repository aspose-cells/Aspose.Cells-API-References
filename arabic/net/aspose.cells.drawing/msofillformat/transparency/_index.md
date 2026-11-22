---
title: "MsoFillFormat.Transparency"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية MsoFillFormat. تُعيد أو تضبط درجة الشفافية للتعبئة المحددة كقيمة من 0.0 غير شفاف إلى 1.0 شفاف"
type: docs
url: /ar/net/aspose.cells.drawing/msofillformat/transparency/
---
## MsoFillFormat.Transparency property

إرجاع أو تعيين درجة الشفافية للملء المحدد كقيمة من 0.0 (معتم) إلى 1.0 (شفاف).

```csharp
public double Transparency { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class MsoFillFormatPropertyTransparencyDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة تعليق إلى الخلية A1
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            comment.Note = "This is a test comment";

            // اضبط خصائص تنسيق التعبئة بما في ذلك الشفافية
            comment.CommentShape.FillFormat.IsVisible = true;
            comment.CommentShape.FillFormat.ForeColor = System.Drawing.Color.Red;
            comment.CommentShape.FillFormat.BackColor = System.Drawing.Color.Yellow;
            
            // اضبط الشفافية (0.0 = غير شفاف تمامًا، 1.0 = شفاف تمامًا)
            comment.CommentShape.FillFormat.Transparency = 0.5;

            // احفظ المصنف
            workbook.Save("CommentTransparencyDemo.xlsx");

            // حمّل دفتر العمل المحفوظ للتحقق من الشفافية
            Workbook verifyWorkbook = new Workbook("CommentTransparencyDemo.xlsx");
            Comment verifyComment = verifyWorkbook.Worksheets[0].Comments[0];
            
            // أخرج قيمة الشفافية لتوضيح أنه تم حفظها وتحميلها بشكل صحيح
            Console.WriteLine("Comment fill transparency: " + 
                verifyComment.CommentShape.FillFormat.Transparency);
        }
    }
}
```

### انظر أيضًا

* class [MsoFillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


