---
title: "TextParagraph.FirstLineIndent"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية TextParagraph. تحدد حجم المسافة البادئة التي ستُطبق على السطر الأول من النص في الفقرة"
type: docs
url: /ar/net/aspose.cells.drawing.texts/textparagraph/firstlineindent/
---
## TextParagraph.FirstLineIndent property

يحدد حجم المسافة البادئة التي سيتم تطبيقها على السطر الأول من النص في الفقرة.

```csharp
public double FirstLineIndent { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextParagraphPropertyFirstLineIndentDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة مربع نص إلى ورقة العمل
            TextBox textBox = worksheet.Shapes.AddTextBox(1, 0, 100, 300, 200, 100);
            textBox.Text = "This is a sample paragraph with multiple lines.\nFirst line should have indent.\nSecond line should be normal.";

            // احصل على فقرة النص من مربع النص
            FontSetting fontSetting = (FontSetting)textBox.GetCharacters()[0];
            TextParagraph textParagraph = (TextParagraph)fontSetting;

            // اعرض قيمة FirstLineIndent الحالية
            Console.WriteLine("Current FirstLineIndent value: " + textParagraph.FirstLineIndent);

            // عيّن قيمة جديدة لـ FirstLineIndent (20 نقطة)
            textParagraph.FirstLineIndent = 20;
            Console.WriteLine("FirstLineIndent set to: " + textParagraph.FirstLineIndent);

            // أضف مربع نص آخر للمقارنة مع المسافة البادئة الافتراضية
            TextBox textBox2 = worksheet.Shapes.AddTextBox(1, 5, 150, 300, 200, 100);
            textBox2.Text = "This is a comparison paragraph without indent.\nFirst line has no indent.\nSecond line is normal.";

            // حفظ المصنف لرؤية التأثيرات
            workbook.Save("TextParagraphPropertyFirstLineIndentDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


