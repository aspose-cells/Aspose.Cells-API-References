---
title: "SettableGlobalizationSettings.GetCommentTitleName"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة SettableGlobalizationSettings. تحصل على اسم عنوان التعليق المعتمد على اللغة وفقًا لنوع عنوان التعليق"
type: docs
url: /ar/net/aspose.cells/settableglobalizationsettings/getcommenttitlename/
---
## SettableGlobalizationSettings.GetCommentTitleName method

يحصل على اسم عنوان التعليق المعتمد على اللغة وفقًا لنوع عنوان التعليق.

```csharp
public override string GetCommentTitleName(CommentTitleType type)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| type | CommentTitleType | نوع عنوان التعليق |

### قيمة الإرجاع

اسم عنوان التعليق المعتمد على اللغة

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class SettableGlobalizationSettingsMethodGetCommentTitleNameWithCommentTitleTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء تعليق في الخلية A1
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            comment.Note = "This is a test comment";
            comment.IsVisible = true;

            // إنشاء إعدادات تعميم مخصصة
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
            
            // تعيين أسماء عناوين تعليقات مخصصة لأنواع مختلفة
            settings.SetCommentTitleName(CommentTitleType.Cell, "Custom Cell Title");
            settings.SetCommentTitleName(CommentTitleType.Comment, "Custom Comment Title");
            settings.SetCommentTitleName(CommentTitleType.Note, "Custom Note Title");
            settings.SetCommentTitleName(CommentTitleType.Reply, "Custom Reply Title");

            // تطبيق إعدادات العولمة على دفتر العمل
            workbook.Settings.GlobalizationSettings = settings;

            try
            {
                // الحصول على وعرض أسماء عناوين التعليقات
                Console.WriteLine("Cell title: " + settings.GetCommentTitleName(CommentTitleType.Cell));
                Console.WriteLine("Comment title: " + settings.GetCommentTitleName(CommentTitleType.Comment));
                Console.WriteLine("Note title: " + settings.GetCommentTitleName(CommentTitleType.Note));
                Console.WriteLine("Reply title: " + settings.GetCommentTitleName(CommentTitleType.Reply));
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetCommentTitleName method: {ex.Message}");
            }

            // احفظ المصنف
            workbook.Save("CommentTitleNamesDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [CommentTitleType](../../../aspose.cells.rendering/commenttitletype/)
* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


