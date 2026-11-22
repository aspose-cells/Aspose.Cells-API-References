---
title: "Shape.LeftInch"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Shape. تمثل الإزاحة الأفقية للشكل من العمود الأيسر بوحدة البوصات"
type: docs
url: /ar/net/aspose.cells.drawing/shape/leftinch/
---
## Shape.LeftInch property

يمثل الإزاحة الأفقية للشكل من عموده الأيسر، بوحدة البوصة.

```csharp
public double LeftInch { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyLeftInchDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف شكلًا نموذجيًا مع جميع المعلمات المطلوبة
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 100, 100);

            // تعيين وإظهار خاصية LeftInch
            shape.LeftInch = 3;
            Console.WriteLine("Shape left position (inches): " + shape.LeftInch);

            // تعديل الموضع الأيسر إذا كان 3 بوصات
            if (shape.LeftInch == 3)
            {
                shape.LeftInch = 1;
                Console.WriteLine("Adjusted shape left position (inches): " + shape.LeftInch);
            }
        }
    }
}
```

### انظر أيضًا

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


