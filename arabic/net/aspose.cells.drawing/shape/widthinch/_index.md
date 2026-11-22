---
title: "Shape.WidthInch"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Shape. تمثل عرض الشكل بوحدة البوصة"
type: docs
url: /ar/net/aspose.cells.drawing/shape/widthinch/
---
## Shape.WidthInch property

يمثل عرض الشكل بوحدة الإنش.

```csharp
public double WidthInch { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyWidthInchDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف شكلاً مستطيلاً مع جميع المعلمات المطلوبة
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 100);

            // تعيين العرض بالبوصات
            shape.WidthInch = 3;
            Console.WriteLine("Shape width (inches): " + shape.WidthInch);

            // تعديل العرض إذا تم استيفاء الشرط
            if (shape.WidthInch == 3)
            {
                shape.WidthInch = 1;
                Console.WriteLine("Modified shape width (inches): " + shape.WidthInch);
            }
        }
    }
}
```

### انظر أيضًا

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


