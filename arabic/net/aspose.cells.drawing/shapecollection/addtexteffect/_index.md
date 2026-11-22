---
title: "ShapeCollection.AddTextEffect"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة ShapeCollection. تُدرج كائن WordArt"
type: docs
url: /ar/net/aspose.cells.drawing/shapecollection/addtexteffect/
---
## ShapeCollection.AddTextEffect method

يدرج كائن WordArt.

```csharp
public Shape AddTextEffect(MsoPresetTextEffect effect, string text, string fontName, int size, 
    bool fontBold, bool fontItalic, int topRow, int top, int leftColumn, int left, int height, 
    int width)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| تأثير | MsoPresetTextEffect | نوع تأثير النص المسبق mso. |
| نص | String | نص WordArt. |
| fontName | String | اسم الخط. |
| الحجم | Int32 | حجم الخط |
| fontBold | منطقي | يشير إلى ما إذا كان الخط عريضًا. |
| fontItalic | منطقي | يشير إلى ما إذا كان الخط مائلًا. |
| topRow | Int32 | فهرس الصف العلوي الأيسر. |
| أعلى | Int32 | يمثل الإزاحة العمودية للشكل من صفه الأيسر، بوحدة البكسل. |
| العمود الأيسر | Int32 | فهرس العمود العلوي الأيسر. |
| يسار | Int32 | يمثل الإزاحة الأفقية للشكل من عموده الأيسر، بوحدة البكسل. |
| الارتفاع | Int32 | يمثل ارتفاع الشكل، بوحدة البكسل. |
| العرض | Int32 | يمثل عرض الشكل، بوحدة البكسل. |

### قيمة الإرجاع

يعيد كائن Shape الذي يمثل كائن WordArt الجديد.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddTextEffectWithMsoPresetTextEffectStringStrinDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            ShapeCollection shapes = worksheet.Shapes;

            Shape wordArt = shapes.AddTextEffect(
                MsoPresetTextEffect.TextEffect10,
                "Sample WordArt",
                "Arial",
                18,
                false,
                false,
                3,
                0,
                3,
                0,
                200,
                50
            );

            workbook.Save("WordArtDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Shape](../../shape/)
* enum [MsoPresetTextEffect](../../msopresettexteffect/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


