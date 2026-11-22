---
title: "Shape.GetLockedProperty"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Shape. تحصل على قيمة الخاصية المقفلة"
type: docs
url: /ar/net/aspose.cells.drawing/shape/getlockedproperty/
---
## Shape.GetLockedProperty method

يحصل على قيمة الخاصية locked.

```csharp
public bool GetLockedProperty(ShapeLockType type)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| type | ShapeLockType | نوع الخاصية المقفلة للشكل. |

### قيمة الإرجاع

يرجع قيمة الخاصية المقفلة.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodGetLockedPropertyWithShapeLockTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة شكل إلى ورقة العمل
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 50);

            // تعيين الخاصية المقفلة لـ AdjustHandles
            shape.SetLockedProperty(ShapeLockType.AdjustHandles, true);

            // التحقق مما إذا كان AdjustHandles مقفلاً
            int noAdjustHandles = 0;
            if (shape.GetLockedProperty(ShapeLockType.AdjustHandles))
                noAdjustHandles = 1;

            Console.WriteLine("AdjustHandles locked status: " + (noAdjustHandles == 1));
        }
    }
}
```

### انظر أيضًا

* enum [ShapeLockType](../../shapelocktype/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


