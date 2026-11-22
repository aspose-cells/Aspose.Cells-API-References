---
title: "TextParagraph.IsHangingPunctuation"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية TextParagraph. تحدد ما إذا كان يجب وضع علامات الترقيم بقوة على سطر النص أو وضعها على سطر مختلف"
type: docs
url: /ar/net/aspose.cells.drawing.texts/textparagraph/ishangingpunctuation/
---
## TextParagraph.IsHangingPunctuation property

يحدد ما إذا كان يجب وضع علامات الترقيم بقوة على سطر النص أو وضعها على سطر نص مختلف.

```csharp
public bool IsHangingPunctuation { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextParagraphPropertyIsHangingPunctuationDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة مربع نص إلى ورقة العمل (تم الإصلاح بإضافة معلمة الارتفاع)
            TextBox textBox = worksheet.Shapes.AddTextBox(0, 0, 200, 100, 200, 100);
            textBox.Text = "This is a sample text with punctuation: \"Hello, world!\"";

            // الحصول على فقرة النص من مربع النص (تم الإصلاح بالتحويل إلى TextParagraph)
            FontSetting fontSetting = (FontSetting)textBox.GetCharacters()[0];
            TextParagraph textParagraph = (TextParagraph)fontSetting;

            // عرض القيمة الحالية لـ IsHangingPunctuation
            Console.WriteLine("Current IsHangingPunctuation value: " + textParagraph.IsHangingPunctuation);

            // تعيين IsHangingPunctuation إلى true
            textParagraph.IsHangingPunctuation = true;
            Console.WriteLine("IsHangingPunctuation set to: " + textParagraph.IsHangingPunctuation);

            // تعيين IsHangingPunctuation إلى false
            textParagraph.IsHangingPunctuation = false;
            Console.WriteLine("IsHangingPunctuation set to: " + textParagraph.IsHangingPunctuation);

            // حفظ المصنف لرؤية التأثيرات (يتطلب فحص بصري)
            workbook.Save("TextParagraphPropertyIsHangingPunctuationDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


