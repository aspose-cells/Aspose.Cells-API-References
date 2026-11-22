---
title: "TextParagraph.Children"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية TextParagraph. تحصل على جميع تشغيلات النص في هذه الفقرة. إذا كانت هذه الفقرة فارغة تُرجع الفقرة نفسها"
type: docs
url: /ar/net/aspose.cells.drawing.texts/textparagraph/children/
---
## TextParagraph.Children property

الحصول على جميع مقاطع النص في هذه الفقرة. إذا كانت هذه الفقرة فارغة، إرجاع الفقرة نفسها.

```csharp
public FontSetting[] Children { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextParagraphPropertyChildrenDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة مربع نص إلى ورقة العمل
            TextBox textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 200, 100, 200);
            textBox.Text = "First line\nSecond line\nThird line";

            // احصل على مجموعة فقرات النص
            FontSetting fontSetting = (FontSetting)textBox.GetCharacters()[0];
            TextParagraph textParagraph = (TextParagraph)fontSetting;

            // اعرض عدد العناصر الفرعية (تشغيلات النص) في الفقرة
            Console.WriteLine("Number of children (text runs): " + textParagraph.Children.Length);

            // عدّل إعدادات الخط لكل عنصر فرعي (تشغيل النص)
            foreach (FontSetting child in textParagraph.Children)
            {
                child.Font.Size = 12;
                child.Font.Color = System.Drawing.Color.Blue;
                child.Font.IsBold = true;
            }

            // أضف سطرًا آخر بتنسيق مختلف
            textBox.Text += "\nFourth line";
            fontSetting = (FontSetting)textBox.GetCharacters()[textBox.Text.Length - 1];
            textParagraph = (TextParagraph)fontSetting;

            // عرض العدد المحدث للأطفال
            Console.WriteLine("Updated number of children: " + textParagraph.Children.Length);

            // احفظ المصنف
            workbook.Save("TextParagraphChildrenDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [FontSetting](../../../aspose.cells/fontsetting/)
* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


