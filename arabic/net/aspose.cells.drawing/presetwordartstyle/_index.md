---
title: "التعداد PresetWordArtStyle"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "التعداد Aspose.Cells.Drawing.PresetWordArtStyle. يمثل أنماط WordArt المحددة مسبقًا"
type: docs
url: /ar/net/aspose.cells.drawing/presetwordartstyle/
---
## PresetWordArtStyle enumeration

يمثل أنماط WordArt المسبقة.

```csharp
public enum PresetWordArtStyle
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| WordArtStyle1 | `1` | ملء - أسود، نص 1، ظل |
| WordArtStyle2 | `2` | ملء - أزرق، تمييز 1، ظل |
| WordArtStyle3 | `3` | ملء - برتقالي، تمييز 2، حدود - تمييز 2 |
| WordArtStyle4 | `4` | ملء - أبيض، حدود - تمييز 1، ظل |
| WordArtStyle5 | `5` | ملء - ذهبي، تمييز 4، حافة مائلة ناعمة |
| WordArtStyle6 | `6` | تعبئة متدرجة - رمادي |
| WordArtStyle7 | `7` | تعبئة متدرجة - أزرق، تمييز 1، انعكاس |
| WordArtStyle8 | `8` | تعبئة متدرجة - ذهبي، تمييز 4، حدود - تمييز 4 |
| WordArtStyle9 | `9` | ملء - أبيض، حدود - تمييز 1، توهج - تمييز 1 |
| WordArtStyle10 | `10` | ملء - رمادي-50٪، تمييز 3، حافة مائلة حادة |
| WordArtStyle11 | `11` | تعبئة - أسود, نص 1, حد - خلفية 1, ظل صلب - خلفية 1 |
| WordArtStyle12 | `12` | تعبئة - أسود, نص 1, حد - خلفية 1, ظل صلب - تدرج 1 |
| WordArtStyle13 | `13` | تعبئة - أزرق, تدرج 1, حد - خلفية 1, ظل صلب - تدرج 1 |
| WordArtStyle14 | `14` | تعبئة - أبيض, حد - تدرج 2, ظل صلب - تدرج 2 |
| WordArtStyle15 | `15` | تعبئة - رمادي-25%, خلفية 2, ظل داخلي |
| WordArtStyle16 | `16` | تعبئة نمط - أبيض, نص 2, قطري صاعد داكن, ظل |
| WordArtStyle17 | `17` | تعبئة نمط - رمادي-50%, تدرج 3, أفقي ضيق, ظل داخلي |
| WordArtStyle18 | `18` | تعبئة - أزرق, تدرج 1, 50%, ظل صلب - تدرج 1 |
| WordArtStyle19 | `19` | تعبئة نمط - أزرق, تدرج 1, قطري هابط فاتح, حد - تدرج 1 |
| WordArtStyle20 | `20` | تعبئة نمط - أزرق-رمادي, نص 2, قطري صاعد داكن, ظل صلب - نص 2 |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class PresetWordArtStyleDemo
    {
        public static void PresetWordArtStyleExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // الوصول إلى مجموعة الأشكال في ورقة العمل
            ShapeCollection shapes = worksheet.Shapes;
            
            // إضافة شكل WordArt بنمط مُعد مسبقًا محدد
            // المعلمات: style, text, upperLeftRow, top, upperLeftColumn, left, height, width
            Shape wordArt = shapes.AddWordArt(PresetWordArtStyle.WordArtStyle2, "Hello Aspose!", 1, 0, 1, 0, 100, 400);
            
            // احفظ المصنف
            workbook.Save("PresetWordArtStyleExample.xlsx");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


