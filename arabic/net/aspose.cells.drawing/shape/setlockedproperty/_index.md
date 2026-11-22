---
title: "Shape.SetLockedProperty"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Shape. اضبط الخاصية المقفلة"
type: docs
url: /ar/net/aspose.cells.drawing/shape/setlockedproperty/
---
## Shape.SetLockedProperty method

يضبط الخاصية locked.

```csharp
public void SetLockedProperty(ShapeLockType type, bool value)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| type | ShapeLockType | النوع المقفل. |
| القيمة | منطقي | قيمة الخاصية. |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodSetLockedPropertyWithShapeLockTypeBooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف شكلًا نموذجيًا مع جميع المعلمات المطلوبة
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 50, 50);

            // وضح استخدام SetLockedProperty
            shape.SetLockedProperty(ShapeLockType.AdjustHandles, true);
            shape.SetLockedProperty(ShapeLockType.Selection, false);

            Console.WriteLine("Shape locked properties set successfully.");
        }
    }
}
```

### انظر أيضًا

* enum [ShapeLockType](../../shapelocktype/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


