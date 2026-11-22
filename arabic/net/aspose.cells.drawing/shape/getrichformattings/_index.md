---
title: "Shape.GetRichFormattings"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Shape. تُرجع جميع كائنات Characters التي تمثل نطاقًا من الأحرف داخل النص"
type: docs
url: /ar/net/aspose.cells.drawing/shape/getrichformattings/
---
## Shape.GetRichFormattings method

يرجع جميع كائنات Characters التي تمثل نطاقًا من الأحرف داخل النص.

```csharp
public FontSetting[] GetRichFormattings()
```

### قيمة الإرجاع

جميع كائنات Characters

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodGetRichFormattingsDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة شكل بنص غني (عدد المعلمات الصحيح لـ AddRectangle)
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 0);
            shape.Text = "This is bold and this is italic";
            
            // تنسيق أجزاء من النص
            shape.Characters(0, 4).Font.IsBold = true;
            shape.Characters(13, 6).Font.IsItalic = true;

            // احصل على تنسيقات النص الغني
            FontSetting[] formattings = shape.GetRichFormattings();

            // عرض معلومات التنسيق
            Console.WriteLine("Rich text formattings:");
            foreach (FontSetting setting in formattings)
            {
                Console.WriteLine($"Text segment: '{shape.Text.Substring(setting.StartIndex, setting.Length)}'");
                Console.WriteLine($"Start index: {setting.StartIndex}");
                Console.WriteLine($"Length: {setting.Length}");
                Console.WriteLine($"Bold: {setting.Font.IsBold}");
                Console.WriteLine($"Italic: {setting.Font.IsItalic}");
                Console.WriteLine();
            }
        }
    }
}
```

### انظر أيضًا

* class [FontSetting](../../../aspose.cells/fontsetting/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


