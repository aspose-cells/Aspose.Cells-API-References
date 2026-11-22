---
title: "تعداد LineSpaceSizeType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "Aspose.Cells.Drawing.Texts.LineSpaceSizeType enum. يمثل نوع الوحدة لحجم تباعد السطر"
type: docs
url: /ar/net/aspose.cells.drawing.texts/linespacesizetype/
---
## LineSpaceSizeType enumeration

يمثل نوع الوحدة لحجم تباعد السطر.

```csharp
public enum LineSpaceSizeType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Percentage | `0` | يمثل بوحدة نسبة مئوية من حجم النص. |
| Points | `1` | يمثل بوحدة نقاط. |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class TextsClassLineSpaceSizeTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة شكل مربع نص
            Shape textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 200);
            
            // تعيين محتوى النص
            textBox.Text = "Sample Text\nSecond Line";
            
            // الوصول إلى الفقرة الأولى في مربع النص
            TextParagraph paragraph = textBox.TextBody.TextParagraphs[0];
            
            // تعيين نوع حجم المسافة بعد إلى نقاط
            paragraph.SpaceAfterSizeType = LineSpaceSizeType.Points;
            
            // تعيين قيمة المسافة بعد (12 نقطة)
            paragraph.SpaceAfter = 12;
            
            // احفظ المصنف
            workbook.Save("output.xlsx");
            
            Console.WriteLine("Text box with line spacing created successfully.");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)


