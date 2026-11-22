---
title: "تعداد LightRigDirectionType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "Aspose.Cells.Drawing.LightRigDirectionType تعداد. يمثل نوع اتجاه إضاءة الجهاز"
type: docs
url: /ar/net/aspose.cells.drawing/lightrigdirectiontype/
---
## LightRigDirectionType enumeration

يمثل نوع اتجاه نظام الإضاءة.

```csharp
public enum LightRigDirectionType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Bottom | `0` | أسفل |
| BottomLeft | `1` | أسفل اليسار. |
| BottomRight | `2` | أسفل يمين. |
| Left | `3` | يسار. |
| Right | `4` | يمين. |
| Top | `5` | أعلى. |
| TopLeft | `6` | أعلى اليسار. |
| TopRight | `7` | أعلى يمين. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class DrawingClassLightRigDirectionTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف شكلاً لتوضيح اتجاه إعداد الإضاءة
            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.TextBox, 10, 10, 200, 200, 0, 0);

            // حدد اتجاه إعداد الإضاءة لتنسيق ثلاثي الأبعاد للشكلة
            shape.ThreeDFormat.LightingDirection = LightRigDirectionType.TopRight;

            // وضح اتجاهات إعداد الإضاءة المختلفة
            Console.WriteLine("Current Light Rig Direction: " + shape.ThreeDFormat.LightingDirection);

            // غيّر اتجاه إعداد الإضاءة
            shape.ThreeDFormat.LightingDirection = LightRigDirectionType.BottomLeft;
            Console.WriteLine("Changed Light Rig Direction: " + shape.ThreeDFormat.LightingDirection);

            // تكرار عبر جميع اتجاهات إعداد الإضاءة الممكنة
            Console.WriteLine("\nAll Light Rig Direction Types:");
            foreach (LightRigDirectionType direction in Enum.GetValues(typeof(LightRigDirectionType)))
            {
                Console.WriteLine(direction.ToString());
            }

            // احفظ المصنف
            workbook.Save("LightRigDirectionTypeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


