---
title: "الفئة TextEffectFormat"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.Drawing.TextEffectFormat. تحتوي على الخصائص والطرق التي تُطبق على كائنات WordArt"
type: docs
url: /ar/net/aspose.cells.drawing/texteffectformat/
---
## TextEffectFormat class

يحتوي على خصائص وطرق تُطبق على كائنات WordArt.

```csharp
public class TextEffectFormat
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [FontBold](../../aspose.cells.drawing/texteffectformat/fontbold/) { get; set; } | يشير إلى ما إذا كان الخط عريضًا. |
| [FontItalic](../../aspose.cells.drawing/texteffectformat/fontitalic/) { get; set; } | يشير إلى ما إذا كان الخط مائلًا. |
| [FontName](../../aspose.cells.drawing/texteffectformat/fontname/) { get; set; } | اسم الخط المستخدم في WordArt. |
| [FontSize](../../aspose.cells.drawing/texteffectformat/fontsize/) { get; set; } | حجم الخط (بالنقاط) المستخدم في WordArt. |
| [PresetShape](../../aspose.cells.drawing/texteffectformat/presetshape/) { get; set; } | يحصل ويضبط نوع الشكل المحدد مسبقًا. |
| [RotatedChars](../../aspose.cells.drawing/texteffectformat/rotatedchars/) { get; set; } | إذا كان صحيحًا، يتم تدوير الأحرف في WordArt المحدد بزاوية 90 درجة بالنسبة إلى الشكل المحيط بـ WordArt. |
| [Text](../../aspose.cells.drawing/texteffectformat/text/) { get; set; } | النص في WordArt. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [SetTextEffect](../../aspose.cells.drawing/texteffectformat/settexteffect/)(MsoPresetTextEffect) | يضبط تأثير النص المحدد مسبقًا. |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassTextEffectFormatDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            ShapeCollection shapes = workbook.Worksheets[0].Shapes;
            
            // إضافة شكل تأثير النص
            shapes.AddTextEffect(MsoPresetTextEffect.TextEffect1, "Aspose", "Arial", 30, false, false, 0, 0, 0, 0, 100, 200);
            
            // تعديل تأثير النص
            TextEffectFormat textEffectFormat = shapes[0].TextEffect;
            textEffectFormat.SetTextEffect(MsoPresetTextEffect.TextEffect10);
            
            // احفظ المصنف
            workbook.Save("TextEffectDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


