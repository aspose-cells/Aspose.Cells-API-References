---
title: "Shape.IsLockAspectRatio"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Shape. True يعني أن نسبة الأبعاد للشكل مقفلة"
type: docs
url: /ar/net/aspose.cells.drawing/shape/islockaspectratio/
---
## Shape.IsLockAspectRatio property

True يعني أن نسبة أبعاد الشكل مقفلة.

```csharp
[Obsolete("Use Shape.IsAspectRatioLocked property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IsLockAspectRatio { get; set; }
```

### ملاحظات

فقط للصور وOle Objects. ملاحظة: هذا العضو الآن غير صالح. بدلاً من ذلك، يرجى استخدام خاصية Shape.IsAspectRatioLocked. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ يوليو 2024. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyIsLockAspectRatioDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف شكلاً مستطيلاً مع جميع المعلمات المطلوبة
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 0);

            // قفل نسبة الأبعاد
            shape.IsLockAspectRatio = true;
            Console.WriteLine("Aspect ratio locked: " + shape.IsLockAspectRatio);

            // إلغاء قفل نسبة الأبعاد
            shape.IsLockAspectRatio = false;
            Console.WriteLine("Aspect ratio locked: " + shape.IsLockAspectRatio);
        }
    }
}
```

### انظر أيضًا

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


