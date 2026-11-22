---
title: "TextOptions.LatinName"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية TextOptions. تحصل وتعيّن الاسم اللاتيني"
type: docs
url: /ar/net/aspose.cells.drawing.texts/textoptions/latinname/
---
## TextOptions.LatinName property

يحصل على الاسم اللاتيني ويضبطه.

```csharp
public string LatinName { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextOptionsPropertyLatinNameDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف شكلاً لعرض خيارات النص
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 150);
            shape.Text = "Sample Text";

            // احصل على TextOptions من الفقرة الأولى للشكل
            TextOptions textOptions = shape.TextBody.TextParagraphs[0].TextOptions;

            // اعرض قيمة LatinName الحالية
            Console.WriteLine("Current LatinName value: " + textOptions.LatinName);

            // عيّن قيمة LatinName جديدة
            textOptions.LatinName = "Times New Roman";

            // أنشئ شكلاً آخر لمقارنة عرض الخط
            Shape shape2 = worksheet.Shapes.AddRectangle(1, 0, 3, 0, 100, 150);
            shape2.Text = "Comparison Text";
            shape2.TextBody.TextParagraphs[0].TextOptions.LatinName = "Arial";

            // حفظ المصنف لرؤية التأثيرات
            workbook.Save("PropertyLatinNameDemo.xlsx");

            // اعرض قيمة LatinName الجديدة
            Console.WriteLine("New LatinName value: " + textOptions.LatinName);
        }
    }
}
```

### انظر أيضًا

* class [TextOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


