---
title: "TextOptions.Kerning"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية TextOptions. تحدد الحد الأدنى لحجم الخط الذي يحدث عنده تقارب الأحرف لهذا تشغيل النص"
type: docs
url: /ar/net/aspose.cells.drawing.texts/textoptions/kerning/
---
## TextOptions.Kerning property

يحدد الحد الأدنى لحجم الخط الذي سيحدث عنده تقليل الفجوة بين الأحرف لهذه مجموعة النص.

```csharp
public double Kerning { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextOptionsPropertyKerningDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف شكلاً يحتوي على نص لعرض تقارب الأحرف
            var shape = worksheet.Shapes.AddTextBox(1, 0, 1, 0, 200, 100);
            shape.Text = "Kerning Demonstration Text";

            // احصل على TextOptions الخاص بالشكل
            TextOptions textOptions = shape.TextOptions;

            // اعرض قيمة تقارب الأحرف الحالية
            Console.WriteLine("Current Kerning value: " + textOptions.Kerning);

            // ضبط التباعد إلى 12 نقطة (الحد الأدنى لحجم الخط لحدوث التباعد)
            textOptions.Kerning = 12;

            // ضبط حجم خط أكبر لملاحظة تأثير التباعد
            textOptions.Size = 24;

            // حفظ المصنف لرؤية التأثير
            workbook.Save("PropertyKerningDemo.xlsx");

            // إنشاء شكل آخر بتباعد مختلف للمقارنة
            var shape2 = worksheet.Shapes.AddTextBox(10, 0, 1, 0, 200, 100);
            shape2.Text = "Comparison Text Without Kerning";
            shape2.TextOptions.Size = 24;
            shape2.TextOptions.Kerning = 0; // No kerning

            // احفظ مرة أخرى مع كلا المثالين
            workbook.Save("PropertyKerningDemoWithComparison.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [TextOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


