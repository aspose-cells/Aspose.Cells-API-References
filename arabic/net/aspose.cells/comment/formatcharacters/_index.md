---
title: "Comment.FormatCharacters"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Comment. تنسيق بعض الأحرف باستخدام إعداد الخط"
type: docs
url: /ar/net/aspose.cells/comment/formatcharacters/
---
## Comment.FormatCharacters method

قم بتنسيق بعض الأحرف باستخدام إعداد الخط.

```csharp
public void FormatCharacters(int startIndex, int length, Font font, StyleFlag flag)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| startIndex | Int32 | فهرس البداية. |
| الطول | Int32 | الطول. |
| خط | خط | إعداد الخط. |
| علامة | StyleFlag | علامة إعداد الخط. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class CommentMethodFormatCharactersWithInt32Int32FontStyleFlagDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة تعليق إلى الخلية A1
            int commentRow = 0;
            int commentColumn = 0;
            Comment comment = worksheet.Comments[commentRow, commentColumn];
            comment.Note = "This is a sample comment with formatted text.";

            // إنشاء خط للتنسيق - تحتاج إلى الحصول عليه من نمط المصنف
            Aspose.Cells.Font font = workbook.CreateStyle().Font;
            font.IsBold = true;
            font.Color = Color.Red;
            font.Size = 14;
            font.Underline = FontUnderlineType.Single;

            // إنشاء علامة النمط لتحديد خصائص الخط التي سيتم تطبيقها
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.FontBold = true;
            styleFlag.FontColor = true;
            styleFlag.FontSize = true;
            styleFlag.FontUnderline = true;

            try
            {
                // تنسيق الأحرف من الفهرس 5، بطول 10
                comment.FormatCharacters(5, 10, font, styleFlag);

                Console.WriteLine("FormatCharacters method executed successfully on the comment.");
                
                // اجعل التعليق مرئياً لرؤية التأثير
                comment.IsVisible = true;
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing FormatCharacters method: {ex.Message}");
            }
            
            // احفظ المصنف
            workbook.Save("CommentFormatCharactersDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Font](../../font/)
* class [StyleFlag](../../styleflag/)
* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


