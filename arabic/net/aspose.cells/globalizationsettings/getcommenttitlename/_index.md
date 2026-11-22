---
title: "GlobalizationSettings.GetCommentTitleName"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة GlobalizationSettings. تحصل على اسم عنوان التعليق المعتمد على اللغة وفقًا لنوع عنوان التعليق"
type: docs
url: /ar/net/aspose.cells/globalizationsettings/getcommenttitlename/
---
## GlobalizationSettings.GetCommentTitleName method

يحصل على اسم عنوان التعليق المعتمد على اللغة وفقًا لنوع عنوان التعليق.

```csharp
public virtual string GetCommentTitleName(CommentTitleType type)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| type | CommentTitleType |  |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class GlobalizationSettingsMethodGetCommentTitleNameWithCommentTitleTypeDemo : GlobalizationSettings
    {
        public override string GetCommentTitleName(CommentTitleType type)
        {
            switch (type)
            {
                case CommentTitleType.Cell:
                    return "Custom Cell Comment";
                case CommentTitleType.Reply:  // Changed from Threaded to Reply
                    return "Custom Threaded Comment";
                default:
                    return base.GetCommentTitleName(type);
            }
        }

        public static void Run()
        {
            Workbook workbook = new Workbook();
            workbook.Settings.GlobalizationSettings = new GlobalizationSettingsMethodGetCommentTitleNameWithCommentTitleTypeDemo(); // Changed to use Settings

            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة تعليق اختبار
            int commentIndex = worksheet.Comments.Add("B5");
            Comment comment = worksheet.Comments[commentIndex];
            comment.Note = "Test comment content";

            try
            {
                // الحصول على عنوان التعليق لأنواع مختلفة
                var cellTitle = workbook.Settings.GlobalizationSettings.GetCommentTitleName(CommentTitleType.Cell); // Changed to use Settings
                var threadedTitle = workbook.Settings.GlobalizationSettings.GetCommentTitleName(CommentTitleType.Reply); // Changed type and Settings

                Console.WriteLine($"Cell Comment Title: {cellTitle}");
                Console.WriteLine($"Threaded Comment Title: {threadedTitle}");

                // تعيين مؤلف التعليق (العنوان) باستخدام إعدادات العولمة المخصصة لدينا
                comment.Author = cellTitle; // Changed from Title to Author
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetCommentTitleName method: {ex.Message}");
            }

            workbook.Save("GetCommentTitleNameDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [CommentTitleType](../../../aspose.cells.rendering/commenttitletype/)
* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


