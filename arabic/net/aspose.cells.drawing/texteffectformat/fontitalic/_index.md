---
title: "TextEffectFormat.FontItalic"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية TextEffectFormat. تشير إلى ما إذا كان الخط مائلًا"
type: docs
url: /ar/net/aspose.cells.drawing/texteffectformat/fontitalic/
---
## TextEffectFormat.FontItalic property

يشير إلى ما إذا كان الخط مائلًا.

```csharp
public bool FontItalic { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TextEffectFormatPropertyFontItalicDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف شكلاً مع تأثير النص
            Shape shape = worksheet.Shapes.AddTextEffect(MsoPresetTextEffect.TextEffect1, "Sample Text", 
                "Arial", 18, false, false, 0, 0, 0, 0, 100, 100);

            // احصل على تنسيق تأثير النص
            TextEffectFormat textEffectFormat = shape.TextEffect;

            // عيّن FontItalic إلى true
            textEffectFormat.FontItalic = true;
            Console.WriteLine("FontItalic after setting to true: " + textEffectFormat.FontItalic);

            // عيّن FontItalic إلى false
            textEffectFormat.FontItalic = false;
            Console.WriteLine("FontItalic after setting to false: " + textEffectFormat.FontItalic);

            // احفظ المصنف
            workbook.Save("TextEffectFormatFontItalicDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [TextEffectFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


