---
title: "Comment.AutoSize"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Comment. تشير إلى ما إذا كان حجم التعليق يتم ضبطه تلقائيًا وفقًا لمحتواه. ملاحظة: في بعض الحالات الخاصة مثل بيئة Mac قد لا يعمل هذا الإعداد. إذا لم يعمل هذا الإعداد يرجى استبداله بـ FitToTextSize"
type: docs
url: /ar/net/aspose.cells/comment/autosize/
---
## Comment.AutoSize property

يشير إلى ما إذا كان حجم التعليق يتم ضبطه تلقائيًا وفقًا لمحتواه. ملاحظة: في بعض الحالات الخاصة (مثل بيئة Mac)، قد لا يكون لهذا الإعداد تأثير. إذا لم يكن لهذا الإعداد تأثير، يرجى استبداله بـ FitToTextSize().

```csharp
public bool AutoSize { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentPropertyAutoSizeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة تعليق إلى الخلية A1
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            comment.Note = "This is a sample comment that will auto-size to fit its content.";

            // ضبط AutoSize إلى true
            comment.AutoSize = true;

            // احفظ المصنف
            workbook.Save("CommentAutoSizeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


