---
title: "Shape.Height"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Shape. تمثل ارتفاع الشكل بوحدة البكسل"
type: docs
url: /ar/net/aspose.cells.drawing/shape/height/
---
## Shape.Height property

يمثل ارتفاع الشكل، بوحدة البكسل.

```csharp
public int Height { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyHeightDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف شكلاً مستطيلاً مع جميع المعلمات المطلوبة
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 100);

            // تعيين الارتفاع الأولي
            shape.Height = 150;
            Console.WriteLine("Initial height: " + shape.Height);

            // تعديل الارتفاع وفقًا للشرط
            if (shape.Height == 150)
            {
                shape.Height = 100;
                Console.WriteLine("Modified height: " + shape.Height);
            }
        }
    }
}
```

### انظر أيضًا

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


