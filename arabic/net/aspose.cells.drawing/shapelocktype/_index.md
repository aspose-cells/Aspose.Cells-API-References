---
title: "تعداد ShapeLockType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "تعداد Aspose.Cells.Drawing.ShapeLockType. يمثل نوع الخاصية التي سيتم قفلها"
type: docs
url: /ar/net/aspose.cells.drawing/shapelocktype/
---
## ShapeLockType enumeration

يمثل نوع الخاصية التي سيتم قفلها.

```csharp
public enum ShapeLockType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Group | `0` | مجموعة |
| AdjustHandles | `1` | ضبط المقابض |
| Text | `2` | نص |
| Points | `3` | نقاط |
| Crop | `4` | قص |
| Selection | `5` | تحديد |
| Move | `6` | نقل |
| AspectRatio | `7` | نسبة الأبعاد |
| Rotation | `8` | دوران |
| Ungroup | `9` | إلغاء التجميع |
| Resize | `10` | تغيير الحجم |
| ShapeType | `11` | نوع الشكل |
| Arrowhead | `12` | رأس السهم |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassShapeLockTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف صورة إلى ورقة العمل
            int index = worksheet.Pictures.Add(0, 0, "example.jpg");
            Aspose.Cells.Drawing.Picture picture = worksheet.Pictures[index];

            // عرض وظيفة ShapeLockType
            picture.SetLockedProperty(Aspose.Cells.Drawing.ShapeLockType.AspectRatio, false);
            bool isAspectRatioLocked = picture.GetLockedProperty(Aspose.Cells.Drawing.ShapeLockType.AspectRatio);

            Console.WriteLine("Aspect Ratio locked: " + isAspectRatioLocked);

            // احفظ المصنف
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


