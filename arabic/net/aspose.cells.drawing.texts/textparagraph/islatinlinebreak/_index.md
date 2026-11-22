---
title: "TextParagraph.IsLatinLineBreak"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية TextParagraph. تحدد ما إذا كان يمكن كسر كلمة لاتينية إلى نصفين وتغليفها إلى السطر التالي دون إضافة شرطة"
type: docs
url: /ar/net/aspose.cells.drawing.texts/textparagraph/islatinlinebreak/
---
## TextParagraph.IsLatinLineBreak property

يحدد ما إذا كان يمكن كسر كلمة لاتينية إلى نصفين وتغليفها إلى السطر التالي دون إضافة شرطة.

```csharp
public bool IsLatinLineBreak { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextParagraphPropertyIsLatinLineBreakDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة مربع نص إلى ورقة العمل (معلمات ثابتة لتضمين الارتفاع)
            TextBox textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 300, 200, 100);
            textBox.Text = "This is a long Latin text that will demonstrate line breaking behavior when IsLatinLineBreak is set to different values.";

            // الحصول على فقرة النص من مربع النص (تمت إضافة تحويل صريح)
            FontSetting fontSetting = (FontSetting)textBox.GetCharacters()[0];
            TextParagraph textParagraph = ((TextParagraph)fontSetting);

            // عرض القيمة الحالية لـ IsLatinLineBreak
            Console.WriteLine("Current IsLatinLineBreak value: " + textParagraph.IsLatinLineBreak);

            // تعيين IsLatinLineBreak إلى false (الكلمات اللاتينية لن تنكسر في نهاية السطر)
            textParagraph.IsLatinLineBreak = false;
            Console.WriteLine("Set IsLatinLineBreak to false - Latin words won't break at line end");
            workbook.Save("LatinLineBreakDisabled.xlsx");

            // تعيين IsLatinLineBreak إلى true (الكلمات اللاتينية يمكن أن تنكسر في نهاية السطر)
            textParagraph.IsLatinLineBreak = true;
            Console.WriteLine("Set IsLatinLineBreak to true - Latin words can break at line end");
            workbook.Save("LatinLineBreakEnabled.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


