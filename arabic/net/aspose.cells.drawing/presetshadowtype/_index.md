---
title: "التعداد PresetShadowType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "التعداد Aspose.Cells.Drawing.PresetShadowType. يمثل نوع الظل المسبق"
type: docs
url: /ar/net/aspose.cells.drawing/presetshadowtype/
---
## PresetShadowType enumeration

يمثل نوع الظل المسبق.

```csharp
public enum PresetShadowType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| NoShadow | `0` | بدون ظل. |
| Custom | `1` | ظل مخصص. |
| OffsetDiagonalBottomRight | `2` | إزاحة الظل الخارجي قطريًا أسفل اليمين. |
| OffsetBottom | `3` | إزاحة الظل الخارجي أسفل. |
| OffsetDiagonalBottomLeft | `4` | إزاحة الظل الخارجي قطري أسفل اليسار. |
| OffsetRight | `5` | إزاحة الظل الخارجي إلى اليمين. |
| OffsetCenter | `6` | إزاحة الظل الخارجي إلى الوسط. |
| OffsetLeft | `7` | إزاحة الظل الخارجي إلى اليسار. |
| OffsetDiagonalTopRight | `8` | إزاحة الظل الخارجي قطري أعلى اليمين. |
| OffsetTop | `9` | إزاحة الظل الخارجي إلى الأعلى. |
| OffsetDiagonalTopLeft | `10` | إزاحة الظل الخارجي قطري أعلى اليسار. |
| InsideDiagonalTopLeft | `11` | ظل داخلي داخل قطري أعلى اليسار. |
| InsideTop | `12` | ظل داخلي داخل الأعلى. |
| InsideDiagonalTopRight | `13` | ظل داخلي داخل قطري أعلى اليمين. |
| InsideLeft | `14` | ظل داخلي داخل اليسار. |
| InsideCenter | `15` | ظل داخلي داخل الوسط. |
| InsideRight | `16` | ظل داخلي داخل اليمين. |
| InsideDiagonalBottomLeft | `17` | ظل داخلي داخل قطري أسفل اليسار. |
| InsideBottom | `18` | ظل داخلي داخل الأسفل. |
| InsideDiagonalBottomRight | `19` | ظل داخلي داخل قطري أسفل اليمين. |
| PerspectiveDiagonalUpperLeft | `20` | ظل خارجي منظور قطري أعلى اليسار. |
| PerspectiveDiagonalUpperRight | `21` | ظل خارجي منظور قطري أعلى اليمين. |
| Below | `22` | ظل خارجي أسفل. |
| PerspectiveDiagonalLowerLeft | `23` | ظل خارجي منظور قطري أسفل اليسار. |
| PerspectiveDiagonalLowerRight | `24` | ظل خارجي منظور قطري أسفل اليمين. |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassPresetShadowTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف شكلاً لتوضيح تأثيرات الظل
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 100);
            
            // حدد أنواع الظل المسبقة المختلفة
            shape.ShadowEffect.PresetType = PresetShadowType.OffsetDiagonalBottomRight;
            Console.WriteLine("Shadow type set to: " + shape.ShadowEffect.PresetType);

            // غيّر إلى نوع ظل آخر
            shape.ShadowEffect.PresetType = PresetShadowType.OffsetBottom;
            Console.WriteLine("Shadow type changed to: " + shape.ShadowEffect.PresetType);

            // احفظ المصنف
            workbook.Save("PresetShadowTypeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


