---
title: "TextEffectFormat.PresetShape"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية TextEffectFormat. تحصل وتضبط نوع الشكل المسبق"
type: docs
url: /ar/net/aspose.cells.drawing/texteffectformat/presetshape/
---
## TextEffectFormat.PresetShape property

يحصل ويضبط نوع الشكل المحدد مسبقًا.

```csharp
public MsoPresetTextEffectShape PresetShape { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TextEffectFormatPropertyPresetShapeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف شكلاً مع تأثير النص
            Shape shape = worksheet.Shapes.AddTextEffect(
                MsoPresetTextEffect.TextEffect1,
                "Sample Text",
                "Arial",
                18,
                false,
                false,
                0,
                0,
                100,
                200,
                0,
                0);

            // احصل على تنسيق تأثير النص
            TextEffectFormat textEffectFormat = shape.TextEffect;

            // تعيين والحصول على خاصية PresetShape
            textEffectFormat.PresetShape = MsoPresetTextEffectShape.ArchUpPour;
            Console.WriteLine("PresetShape: " + textEffectFormat.PresetShape);

            // تعديل الخصائص الأخرى
            textEffectFormat.Text = "Updated Text";
            textEffectFormat.FontBold = true;
            textEffectFormat.FontSize = 24;

            // احفظ المصنف
            workbook.Save("TextEffectFormatDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [MsoPresetTextEffectShape](../../msopresettexteffectshape/)
* class [TextEffectFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


