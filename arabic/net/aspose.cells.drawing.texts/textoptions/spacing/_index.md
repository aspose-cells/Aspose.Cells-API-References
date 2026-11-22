---
title: "TextOptions.Spacing"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية TextOptions. تحدد التباعد بين الأحرف داخل مقطع نصي"
type: docs
url: /ar/net/aspose.cells.drawing.texts/textoptions/spacing/
---
## TextOptions.Spacing property

يحدد المسافة بين الأحرف داخل مجموعة النص.

```csharp
public double Spacing { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextOptionsPropertySpacingDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة مربع نص إلى ورقة العمل
            TextBox textBox = worksheet.Shapes.AddTextBox(0, 0, 2, 0, 100, 200);
            textBox.Text = "Sample Text with Spacing";

            // احصل على خيارات النص لمربع النص
            TextOptions textOptions = textBox.TextOptions;

            // اعرض قيمة التباعد الحالية
            Console.WriteLine("Current Spacing value: " + textOptions.Spacing);

            // اضبط قيم التباعد الجديدة وشاهد التأثيرات
            textOptions.Spacing = 2.0; // Increased spacing
            Console.WriteLine("Text with increased spacing (2.0)");

            // احفظ المصنف مع التباعد الأول
            workbook.Save("TextSpacingDemo1.xlsx");

            // غيّر التباعد إلى قيمة سلبية (الأحرف أقرب إلى بعضها)
            textOptions.Spacing = -1.0;
            Console.WriteLine("Text with decreased spacing (-1.0)");

            // احفظ المصنف مع التباعد الثاني
            workbook.Save("TextSpacingDemo2.xlsx");

            // إعادة الضبط إلى التباعد الافتراضي
            textOptions.Spacing = 0.0;
            Console.WriteLine("Text with default spacing (0.0)");

            // احفظ المصنف مع التباعد الافتراضي
            workbook.Save("TextSpacingDemo3.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [TextOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


