---
title: "ShapeCollection.AddWordArt"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة ShapeCollection. تُضيف WordArt مسبق الإعداد منذ Excel 2007."
type: docs
url: /ar/net/aspose.cells.drawing/shapecollection/addwordart/
---
## ShapeCollection.AddWordArt method

يضيف WordArt مسبق الإعداد منذ Excel 2007.s

```csharp
public Shape AddWordArt(PresetWordArtStyle style, string text, int topRow, int top, int leftColumn, 
    int left, int height, int width)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| النمط | PresetWordArtStyle | نمط WordArt المسبق الإعداد. |
| نص | String | النص. |
| topRow | Int32 | فهرس الصف العلوي الأيسر. |
| أعلى | Int32 | يمثل الإزاحة العمودية للشكل من صفه الأيسر، بوحدة البكسل. |
| العمود الأيسر | Int32 | فهرس العمود العلوي الأيسر. |
| يسار | Int32 | يمثل الإزاحة الأفقية للشكل من عموده الأيسر، بوحدة البكسل. |
| الارتفاع | Int32 | يمثل ارتفاع الشكل، بوحدة البكسل. |
| العرض | Int32 | يمثل عرض الشكل، بوحدة البكسل. |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddWordArtWithPresetWordArtStyleStringInt32IDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // احصل على مجموعة الأشكال
            ShapeCollection shapes = worksheet.Shapes;

            // أضف WordArt مع المعلمات المحددة
            Shape wordArt = shapes.AddWordArt(
                PresetWordArtStyle.WordArtStyle1, 
                "Sample WordArt", 
                10,  // left
                10,  // top
                200, // width
                50,  // height
                100, // rotation
                200  // z-order
            );

            // احفظ المصنف
            workbook.Save("WordArtDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Shape](../../shape/)
* enum [PresetWordArtStyle](../../presetwordartstyle/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


