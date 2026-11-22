---
title: "فئة Comment"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "فئة Aspose.Cells.Comment. تغلف الكائن الذي يمثل تعليق الخلية"
type: docs
url: /ar/net/aspose.cells/comment/
---
## Comment class

يغلف الكائن الذي يمثل تعليق خلية.

```csharp
public class Comment
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Author](../../aspose.cells/comment/author/) { get; set; } | يحصل ويضبط اسم مؤلف التعليق الأصلي |
| [AutoSize](../../aspose.cells/comment/autosize/) { get; set; } | يشير إلى ما إذا كان حجم التعليق يتم ضبطه تلقائيًا وفقًا لمحتواه. ملاحظة: في بعض الحالات الخاصة (مثل بيئة Mac)، قد لا يكون لهذا الإعداد تأثير. إذا لم يكن لهذا الإعداد تأثير، يرجى استبداله بـ FitToTextSize(). |
| [Column](../../aspose.cells/comment/column/) { get; } | يحصل على فهرس العمود للتعليق. |
| [CommentShape](../../aspose.cells/comment/commentshape/) { get; } | احصل على كائن Shape الذي يمثل الشكل المرفق بالتعليق المحدد. |
| [Font](../../aspose.cells/comment/font/) { get; } | يحصل على خط التعليق. |
| [Height](../../aspose.cells/comment/height/) { get; set; } | يمثل ارتفاع التعليق، بوحدة البكسل. |
| [HeightCM](../../aspose.cells/comment/heightcm/) { get; set; } | يمثل ارتفاع التعليق، بوحدة السنتيمتر. |
| [HeightInch](../../aspose.cells/comment/heightinch/) { get; set; } | يمثل ارتفاع التعليق، بوحدة الإنش. |
| [HtmlNote](../../aspose.cells/comment/htmlnote/) { get; set; } | يحصل ويضبط سلسلة html التي تحتوي على البيانات وبعض التنسيقات في هذا التعليق. |
| [IsThreadedComment](../../aspose.cells/comment/isthreadedcomment/) { get; } | يشير إلى ما إذا كان هذا التعليق تعليقًا متسلسلًا. |
| [IsVisible](../../aspose.cells/comment/isvisible/) { get; set; } | يمثل ما إذا كان التعليق مرئيًا أم لا. |
| [Note](../../aspose.cells/comment/note/) { get; set; } | يمثل محتوى التعليق. |
| [Row](../../aspose.cells/comment/row/) { get; } | يحصل على فهرس الصف للتعليق. |
| [TextHorizontalAlignment](../../aspose.cells/comment/texthorizontalalignment/) { get; set; } | يحصل ويضبط نوع محاذاة النص الأفقية للتعليق. |
| [TextOrientationType](../../aspose.cells/comment/textorientationtype/) { get; set; } | يحصل ويضبط نوع توجيه النص للتعليق. |
| [TextVerticalAlignment](../../aspose.cells/comment/textverticalalignment/) { get; set; } | يحصل ويضبط نوع محاذاة النص العمودية للتعليق. |
| [ThreadedComments](../../aspose.cells/comment/threadedcomments/) { get; } | يحصل على قائمة التعليقات المتسلسلة؛ |
| [Width](../../aspose.cells/comment/width/) { get; set; } | يمثل عرض التعليق، بوحدة البكسل. |
| [WidthCM](../../aspose.cells/comment/widthcm/) { get; set; } | يمثل عرض التعليق، بوحدة السنتيمتر. |
| [WidthInch](../../aspose.cells/comment/widthinch/) { get; set; } | يمثل عرض التعليق، بوحدة الإنش. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [Characters](../../aspose.cells/comment/characters/)(int, int) | يرجع كائن Characters يمثل نطاقًا من الأحرف داخل نص التعليق. |
| [FormatCharacters](../../aspose.cells/comment/formatcharacters/)(int, int, Font, StyleFlag) | قم بتنسيق بعض الأحرف باستخدام إعداد الخط. |
| [GetRichFormattings](../../aspose.cells/comment/getrichformattings/)() | يرجع جميع كائنات Characters التي تمثل نطاقًا من الأحرف داخل نص التعليق. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class CommentDemo
    {
        public static void CommentExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            // الوصول إلى مجموعة التعليقات في ورقة العمل
            CommentCollection comments = worksheet.Comments;

            // إضافة تعليق إلى الخلية A1
            int commentIndex1 = comments.Add(0, 0);
            Comment comment1 = comments[commentIndex1];
            comment1.Note = "First note.";
            comment1.Font.Name = "Times New Roman";
            comment1.Font.Size = 12;
            comment1.Font.Color = System.Drawing.Color.Red;
            comment1.Author = "Carl.Yang";
            comment1.HtmlNote = "<Font Style='FONT-FAMILY: Calibri;FONT-SIZE: 11pt;COLOR: #0000ff;TEXT-ALIGN: left;'>This is a <b>test</b>.</Font>";
            comment1.IsVisible = true;
            comment1.TextOrientationType = TextOrientationType.TopToBottom;
            comment1.TextHorizontalAlignment = TextAlignmentType.Center;
            comment1.TextVerticalAlignment = TextAlignmentType.Center;
            comment1.AutoSize = true;
            comment1.HeightCM = 1.0;
            comment1.WidthCM = 1.0;
            comment1.Width = 10;
            comment1.Height = 10;
            comment1.WidthInch = 1.0;
            comment1.HeightInch = 1.0;

            // الوصول إلى شكل التعليق
            CommentShape shape = comment1.CommentShape;
            int w = shape.Width;
            int h = shape.Height;

            // إضافة تعليق إلى الخلية B2
            comments.Add("B2");
            Comment comment2 = comments["B2"];
            comment2.Note = "Second note.";

            // احفظ المصنف
            workbook.Save("CommentExample.xlsx");
            workbook.Save("CommentExample.pdf");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


