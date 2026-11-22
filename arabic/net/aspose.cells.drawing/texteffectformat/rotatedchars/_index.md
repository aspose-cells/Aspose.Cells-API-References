---
title: "TextEffectFormat.RotatedChars"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية TextEffectFormat. إذا كانت true، تُدوَّر الأحرف في WordArt المحدد بزاوية 90 درجة بالنسبة إلى الشكل المحيط بـ WordArt"
type: docs
url: /ar/net/aspose.cells.drawing/texteffectformat/rotatedchars/
---
## TextEffectFormat.RotatedChars property

إذا كان صحيحًا، يتم تدوير الأحرف في WordArt المحدد بزاوية 90 درجة بالنسبة إلى الشكل المحيط بـ WordArt.

```csharp
public bool RotatedChars { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TextEffectFormatPropertyRotatedCharsDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف شكلاً مع تأثير النص
            Shape shape = worksheet.Shapes.AddTextEffect(MsoPresetTextEffect.TextEffect1, "Sample Text", 
                "Arial", 18, false, false, 0, 0, 100, 100, 200, 50);

            // احصل على تنسيق تأثير النص
            TextEffectFormat textEffectFormat = shape.TextEffect;

            // عيّن خاصية RotatedChars إلى true
            textEffectFormat.RotatedChars = true;

            // احفظ المصنف
            workbook.Save("TextEffectFormat_RotatedChars_Output.xlsx");

            // تحقق من خاصية RotatedChars
            Console.WriteLine("RotatedChars property value: " + textEffectFormat.RotatedChars);
        }
    }
}
```

### انظر أيضًا

* class [TextEffectFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


