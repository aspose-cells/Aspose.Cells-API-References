---
title: "SettableGlobalizationSettings.SetCommentTitleName"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة SettableGlobalizationSettings. تحصل على اسم عنوان التعليق المعتمد على اللغة وفقًا لنوع عنوان التعليق"
type: docs
url: /ar/net/aspose.cells/settableglobalizationsettings/setcommenttitlename/
---
## SettableGlobalizationSettings.SetCommentTitleName method

يحصل على اسم عنوان التعليق المعتمد على اللغة وفقًا لنوع عنوان التعليق.

```csharp
public void SetCommentTitleName(CommentTitleType type, string name)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| type | CommentTitleType | نوع عنوان التعليق |
| name | String | اسم عنوان التعليق المعتمد على اللغة |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class SettableGlobalizationSettingsMethodSetCommentTitleNameWithCommentTitleTypeStringDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة تعليق إلى الخلية A1
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            comment.Note = "This is a sample comment";
            comment.IsVisible = true;

            // أنشئ إعدادات العولمة
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();

            try
            {
                // تعيين أسماء عناوين تعليقات مخصصة لأنواع مختلفة
                settings.SetCommentTitleName(CommentTitleType.Cell, "Custom Cell Title");
                settings.SetCommentTitleName(CommentTitleType.Comment, "Custom Comment Title");
                settings.SetCommentTitleName(CommentTitleType.Note, "Custom Note Title");
                settings.SetCommentTitleName(CommentTitleType.Reply, "Custom Reply Title");

                // تطبيق إعدادات العولمة على دفتر العمل
                workbook.Settings.GlobalizationSettings = settings;

                Console.WriteLine("SetCommentTitleName method executed successfully with parameters (CommentTitleType, String)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetCommentTitleName method: {ex.Message}");
            }

            // احفظ المصنف
            workbook.Save("MethodSetCommentTitleNameDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [CommentTitleType](../../../aspose.cells.rendering/commenttitletype/)
* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


