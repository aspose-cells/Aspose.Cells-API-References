---
title: "Comment.Characters"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Comment. تُرجع كائن Characters يمثل نطاقًا من الأحرف داخل نص التعليق"
type: docs
url: /ar/net/aspose.cells/comment/characters/
---
## Comment.Characters method

يرجع كائن Characters يمثل نطاقًا من الأحرف داخل نص التعليق.

```csharp
public FontSetting Characters(int startIndex, int length)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| startIndex | Int32 | فهرس بداية الحرف. |
| الطول | Int32 | عدد الأحرف. |

### قيمة الإرجاع

كائن الأحرف.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentMethodCharactersWithInt32Int32Demo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة تعليق إلى الخلية A1
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment1 = worksheet.Comments[commentIndex];
            comment1.Note = "This is a sample comment";
            
            // احصل على إعداد الخط لأول 4 أحرف
            FontSetting fontSetting = comment1.Characters(0, 4);
            
            // عدّل إعدادات الخط
            fontSetting.Font.Color = System.Drawing.Color.Red;
            fontSetting.Font.IsBold = true;
            
            // احفظ المصنف
            workbook.Save("CommentFontSettingDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [FontSetting](../../fontsetting/)
* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


