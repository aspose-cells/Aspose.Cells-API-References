---
title: "التعداد MsoPresetTextEffectShape"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "التعداد Aspose.Cells.Drawing.MsoPresetTextEffectShape. يمثل نوع شكل تأثير النص المحدد مسبقاً في WordArt"
type: docs
url: /ar/net/aspose.cells.drawing/msopresettexteffectshape/
---
## MsoPresetTextEffectShape enumeration

يمثل نوع شكل تأثير النص المسبق في WordArt.

```csharp
public enum MsoPresetTextEffectShape
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| PlainText | `136` | نص عادي |
| Stop | `137` | إيقاف |
| TriangleUp | `138` | مثلث لأعلى |
| TriangleDown | `139` | مثلث لأسفل |
| ChevronUp | `140` | شيفرون لأعلى |
| ChevronDown | `141` | شيفرون لأسفل |
| RingInside | `142` | حلقة داخلية |
| RingOutside | `143` | حلقة خارجية |
| ArchUpCurve | `144` | قوس لأعلى منحني |
| ArchDownCurve | `145` | قوس لأسفل منحني |
| CircleCurve | `146` | منحنى دائري |
| ButtonCurve | `147` | منحنى زر |
| ArchUpPour | `148` | قوس صب لأعلى |
| ArchDownPour | `149` | قوس صب لأسفل |
| CirclePour | `150` | صب دائري |
| ButtonPour | `151` | صب زر |
| CurveUp | `152` | منحنى لأعلى |
| CurveDown | `153` | منحنى لأسفل |
| CanUp | `174` | علبة لأعلى |
| CanDown | `175` | علبة لأسفل |
| Wave1 | `156` | موجة 1 |
| Wave2 | `157` | موجة 2 |
| DoubleWave1 | `158` | موجة مزدوجة 1 |
| DoubleWave2 | `159` | موجة مزدوجة 2 |
| Inflate | `160` | انتفاخ |
| Deflate | `161` | تقليل |
| InflateBottom | `162` | توسيع أسفل |
| DeflateBottom | `163` | تقليل أسفل |
| InflateTop | `164` | توسيع أعلى |
| DeflateTop | `165` | تقليل أعلى |
| DeflateInflate | `166` | تقليل وتوسيع |
| DeflateInflateDeflate | `167` | تقليل وتوسيع وتقليل |
| FadeRight | `168` | تلاشي يمين |
| FadeLeft | `169` | تلاشي يسار |
| FadeUp | `170` | تلاشي أعلى |
| FadeDown | `171` | تلاشي أسفل |
| SlantUp | `172` | انحدار أعلى |
| SlantDown | `173` | انحدار أسفل |
| CascadeUp | `154` | تسلسل أعلى |
| CascadeDown | `155` | تسلسل أسفل |
| Mixed | `255` | مختلط |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class MsoPresetTextEffectShapeDemo
    {
        public static void MsoPresetTextEffectShapeExample()
        {
            // إنشاء كائن Workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            ShapeCollection shapes = worksheet.Shapes;

            // إضافة شكل تأثير نص WordArt
            shapes.AddTextEffect(MsoPresetTextEffect.TextEffect1, "Aspose", "Arial", 30, false, false, 0, 0, 0, 0, 100, 200);
            TextEffectFormat textEffectFormat = shapes[0].TextEffect;

            // تعيين نوع الشكل المسبق
            textEffectFormat.PresetShape = MsoPresetTextEffectShape.ArchUpCurve;

            // احفظ المصنف
            workbook.Save("MsoPresetTextEffectShapeExample.xlsx");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


