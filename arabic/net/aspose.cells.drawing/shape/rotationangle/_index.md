---
title: "Shape.RotationAngle"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Shape. تسترجع وتضبط دوران الشكل"
type: docs
url: /ar/net/aspose.cells.drawing/shape/rotationangle/
---
## Shape.RotationAngle property

يحصل على ويضبط دوران الشكل.

```csharp
public double RotationAngle { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyRotationAngleDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف شكلاً مستطيلاً مع جميع المعلمات المطلوبة
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 100, 200, 0, 0);

            // ضبط زاوية الدوران إلى 60 درجة
            shape.RotationAngle = 60;
            Console.WriteLine("Shape rotation angle set to: " + shape.RotationAngle);

            // الحصول على زاوية الدوران الحالية
            double currentAngle = shape.RotationAngle;
            Console.WriteLine("Current shape rotation angle: " + currentAngle);

            // احفظ المصنف
            workbook.Save("ShapeRotationDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


