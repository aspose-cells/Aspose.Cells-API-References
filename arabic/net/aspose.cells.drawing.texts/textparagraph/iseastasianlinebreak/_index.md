---
title: "TextParagraph.IsEastAsianLineBreak"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية TextParagraph. تحدد ما إذا كان يمكن كسر كلمة شرق آسيوية إلى نصفين وتغليفها إلى السطر التالي دون إضافة شرطة"
type: docs
url: /ar/net/aspose.cells.drawing.texts/textparagraph/iseastasianlinebreak/
---
## TextParagraph.IsEastAsianLineBreak property

يحدد ما إذا كان يمكن كسر كلمة شرق آسيوية إلى نصفين وتغليفها إلى السطر التالي دون إضافة شرطة.

```csharp
public bool IsEastAsianLineBreak { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextParagraphPropertyIsEastAsianLineBreakDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة مربع نص إلى ورقة العمل
            TextBox textBox = worksheet.Shapes.AddTextBox(1, 0, 1, 0, 200, 200);
            textBox.Text = "これは東アジアのテキストの例です。This is Latin text example.";

            // الحصول على فقرة النص من الفقرة الأولى لمربع النص
            TextParagraph paragraph = textBox.TextBody.TextParagraphs[0];

            // اعرض القيمة الحالية لـ IsEastAsianLineBreak
            Console.WriteLine("Current IsEastAsianLineBreak value: " + paragraph.IsEastAsianLineBreak);

            // ضبط IsEastAsianLineBreak إلى false (يمكن كسر الكلمات شرق آسيوية)
            paragraph.IsEastAsianLineBreak = false;
            Console.WriteLine("After setting IsEastAsianLineBreak to false, text may break East Asian words.");

            // احفظ المصنف مع تعطيل فاصل السطر شرق آسيوي
            workbook.Save("EastAsianLineBreakDisabled.xlsx");

            // ضبط IsEastAsianLineBreak إلى true (لن يتم كسر الكلمات شرق آسيوية)
            paragraph.IsEastAsianLineBreak = true;
            Console.WriteLine("After setting IsEastAsianLineBreak to true, text won't break East Asian words.");

            // احفظ المصنف مع تمكين فاصل السطر شرق آسيوي
            workbook.Save("EastAsianLineBreakEnabled.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


