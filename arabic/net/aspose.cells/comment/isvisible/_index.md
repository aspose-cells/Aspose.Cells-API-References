---
title: "Comment.IsVisible"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Comment. تمثل ما إذا كان التعليق مرئياً أم لا"
type: docs
url: /ar/net/aspose.cells/comment/isvisible/
---
## Comment.IsVisible property

يمثل ما إذا كان التعليق مرئيًا أم لا.

```csharp
public bool IsVisible { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentPropertyIsVisibleDemo
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

            // اجعل التعليق مرئياً
            comment.IsVisible = true;

            // تحقق مما إذا كان التعليق مرئياً
            if (comment.IsVisible)
            {
                Console.WriteLine("The comment is visible");
            }

            // احفظ المصنف
            workbook.Save("CommentVisibilityDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


