---
title: "TextParagraph.FontAlignType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية TextParagraph. تحدد موضع الكلمات الفعلية عمودياً على سطر النص. يتعامل هذا مع وضعية الأحرف عمودياً بالنسبة لخطوط الأساس"
type: docs
url: /ar/net/aspose.cells.drawing.texts/textparagraph/fontaligntype/
---
## TextParagraph.FontAlignType property

يحدد موضع الكلمات الفعلية عموديًا على سطر النص. يتعامل هذا مع وضعية الأحرف عموديًا بالنسبة للخط الأساسي.

```csharp
public TextFontAlignType FontAlignType { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextParagraphPropertyFontAlignTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة مربع نص إلى ورقة العمل
            int textboxIndex = worksheet.TextBoxes.Add(1, 1, 200, 400);
            TextBox textbox = worksheet.TextBoxes[textboxIndex];
            textbox.Text = "Sample Text\nFor Font Alignment Demo";

            // احصل على الفقرة الأولى من مربع النص
            TextParagraph paragraph = textbox.TextBody.TextParagraphs[0];

            // اعرض القيمة الحالية لـ FontAlignType
            Console.WriteLine("Current FontAlignType value: " + paragraph.FontAlignType);

            // ضبط FontAlignType إلى الأسفل
            paragraph.FontAlignType = TextFontAlignType.Bottom;
            Console.WriteLine("FontAlignType set to: " + paragraph.FontAlignType);

            // ضبط FontAlignType إلى الوسط
            paragraph.FontAlignType = TextFontAlignType.Center;
            Console.WriteLine("FontAlignType set to: " + paragraph.FontAlignType);

            // ضبط FontAlignType إلى الأعلى
            paragraph.FontAlignType = TextFontAlignType.Top;
            Console.WriteLine("FontAlignType set to: " + paragraph.FontAlignType);

            // حفظ المصنف لرؤية التأثيرات
            workbook.Save("TextParagraphPropertyFontAlignTypeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [TextFontAlignType](../../textfontaligntype/)
* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


