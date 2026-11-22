---
title: "Shape.TextEffect"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية الشكل. تُرجع كائن TextEffectFormat يحتوي على خصائص تنسيق تأثير النص للشكل المحدد. ينطبق على كائنات Shape التي تمثل WordArt"
type: docs
url: /ar/net/aspose.cells.drawing/shape/texteffect/
---
## Shape.TextEffect property

تُرجع كائن TextEffectFormat يحتوي على خصائص تنسيق تأثير النص للشكل المحدد. ينطبق على كائنات Shape التي تمثل WordArt.

```csharp
public TextEffectFormat TextEffect { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyTextEffectDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف شكل WordArt مع المعلمات الصحيحة
            Shape shape = worksheet.Shapes.AddWordArt(PresetWordArtStyle.WordArtStyle1, "Sample Text", 10, 10, 200, 50, 0, 0);

            // تحقق مما إذا كان WordArt وابدأ بالوصول إلى خصائص TextEffect
            if (shape.IsWordArt)
            {
                TextEffectFormat textEffectFormat = shape.TextEffect;
                textEffectFormat.FontBold = true;
                textEffectFormat.FontItalic = true;
                textEffectFormat.FontName = "Arial";
                textEffectFormat.FontSize = 14;
            }

            // احفظ المصنف
            workbook.Save("TextEffectDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [TextEffectFormat](../../texteffectformat/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


