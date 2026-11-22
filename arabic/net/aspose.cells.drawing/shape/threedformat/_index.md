---
title: "Shape.ThreeDFormat"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Shape. تحصل وتعيّن تنسيق ثلاثي الأبعاد للشكل"
type: docs
url: /ar/net/aspose.cells.drawing/shape/threedformat/
---
## Shape.ThreeDFormat property

يحصل ويضبط تنسيق ثلاثي الأبعاد للشكل.

```csharp
public ThreeDFormat ThreeDFormat { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyThreeDFormatDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف شكلًا نموذجيًا مع جميع المعلمات المطلوبة
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 100);

            // الوصول إلى خصائص تنسيق ثلاثي الأبعاد وتعديلها
            ThreeDFormat threeDFormat = shape.ThreeDFormat;
            threeDFormat.ExtrusionColor.Color = System.Drawing.Color.Blue;
            threeDFormat.LightAngle = 45;
            threeDFormat.ContourWidth = 2;
            threeDFormat.ContourColor.Color = System.Drawing.Color.Red;

            // احفظ المصنف
            workbook.Save("ThreeDFormatDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ThreeDFormat](../../threedformat/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


