---
title: "Shape.HeightInch"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Shape. تمثل ارتفاع الشكل بوحدة البوصة"
type: docs
url: /ar/net/aspose.cells.drawing/shape/heightinch/
---
## Shape.HeightInch property

يمثل ارتفاع الشكل، بوحدة البوصة.

```csharp
public double HeightInch { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyHeightInchDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف شكلاً مستطيلاً مع جميع المعلمات المطلوبة
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 100);

            // اضبط واحصل على الارتفاع بوحدة البوصة
            shape.HeightInch = 3;
            Console.WriteLine("Shape height (inches): " + shape.HeightInch);

            // عدّل الارتفاع إذا تم استيفاء الشرط
            if (shape.HeightInch == 3)
            {
                shape.HeightInch = 1;
                Console.WriteLine("Modified shape height (inches): " + shape.HeightInch);
            }
        }
    }
}
```

### انظر أيضًا

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


