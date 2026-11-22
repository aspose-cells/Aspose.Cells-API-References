---
title: "Enum BevelType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "Aspose.Cells.Drawing.BevelType enum. يمثل إعدادًا مسبقًا لنوع الحافة التي يمكن تطبيقها على شكل ثلاثي الأبعاد"
type: docs
url: /ar/net/aspose.cells.drawing/beveltype/
---
## BevelType enumeration

يمثل إعدادًا مسبقًا لنوع الحافة التي يمكن تطبيقها على شكل ثلاثي الأبعاد.

```csharp
public enum BevelType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| None | `0` | بدون حافة |
| Angle | `1` | زاوية |
| ArtDeco | `2` | آرت ديكو |
| Circle | `3` | دائرة |
| Convex | `4` | محدب |
| CoolSlant | `5` | انحدار أنيق |
| Cross | `6` | صليب |
| Divot | `7` | ثقب |
| HardEdge | `8` | حافة صلبة |
| RelaxedInset | `9` | إدراج مريح |
| Riblet | `10` | خط رفيع |
| Slope | `11` | منحدر |
| SoftRound | `12` | دائري ناعم |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class BevelTypeDemo
    {
        public static void BevelTypeExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة شكل إلى ورقة العمل
            var shape = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 2, 0, 2, 0, 100, 100);

            // الوصول إلى تنسيق ثلاثي الأبعاد للشكل
            ThreeDFormat threeDFormat = shape.ThreeDFormat;

            // تعيين نوع الحافة العلوية وأبعادها
            threeDFormat.TopBevelType = BevelType.SoftRound;
            threeDFormat.TopBevelWidth = 10;
            threeDFormat.TopBevelHeight = 10;

            // تعيين نوع الحافة السفلية وأبعادها
            threeDFormat.BottomBevelType = BevelType.Divot;
            threeDFormat.BottomBevelWidth = 5;
            threeDFormat.BottomBevelHeight = 5;

            // احفظ المصنف
            workbook.Save("BevelTypeExample.xlsx");
            workbook.Save("BevelTypeExample.pdf");

            return;
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


