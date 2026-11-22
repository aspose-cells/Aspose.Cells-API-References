---
title: "تعداد CommentTitleType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "تعداد Aspose.Cells.Rendering.CommentTitleType. يمثل نوع عنوان التعليق أثناء العرض عندما يتم ضبط التعليق ليظهر في نهاية الورقة"
type: docs
url: /ar/net/aspose.cells.rendering/commenttitletype/
---
## CommentTitleType enumeration

يمثل نوع عنوان التعليق أثناء العرض عندما يتم ضبط التعليق ليظهر في نهاية الورقة.

```csharp
public enum CommentTitleType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Cell | `0` | يمثل خلية عنوان التعليق. |
| Comment | `1` | يمثل تعليق عنوان التعليق. |
| Note | `2` | يمثل ملاحظة عنوان التعليق. |
| Reply | `3` | يمثل رد عنوان التعليق. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class RenderingClassCommentTitleTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد للعرض
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // إنشاء إعدادات تعميم مخصصة
                SettableGlobalizationSettings globalizationSettings = new SettableGlobalizationSettings();

                // عرض جميع قيم تعداد CommentTitleType
                Console.WriteLine("Available CommentTitleType values:");
                Console.WriteLine($"Cell: {(int)CommentTitleType.Cell}");
                Console.WriteLine($"Comment: {(int)CommentTitleType.Comment}");
                Console.WriteLine($"Note: {(int)CommentTitleType.Note}");
                Console.WriteLine($"Reply: {(int)CommentTitleType.Reply}");

                // تعيين عناوين مخصصة لكل نوع من التعليقات
                globalizationSettings.SetCommentTitleName(CommentTitleType.Cell, "Custom Cell Title");
                globalizationSettings.SetCommentTitleName(CommentTitleType.Comment, "Custom Comment Title");
                globalizationSettings.SetCommentTitleName(CommentTitleType.Note, "Custom Note Title");
                globalizationSettings.SetCommentTitleName(CommentTitleType.Reply, "Custom Reply Title");

                // تطبيق إعدادات العولمة على دفتر العمل
                workbook.Settings.GlobalizationSettings = globalizationSettings;

                // إضافة تعليق لعرض الوظيفة
                int commentIndex = worksheet.Comments.Add("A1");
                Comment comment = worksheet.Comments[commentIndex];
                comment.Note = "This is a test comment";
                comment.Author = "Test Author";

                // احفظ المصنف
                workbook.Save("CommentTitleTypeDemo.xlsx");

                Console.WriteLine("CommentTitleType demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in CommentTitleType demonstration: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


