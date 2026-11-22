---
title: "Shape.HeightCM"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Shape. تمثل ارتفاع الشكل بوحدة السنتيمترات"
type: docs
url: /ar/net/aspose.cells.drawing/shape/heightcm/
---
## Shape.HeightCM property

يمثل ارتفاع الشكل، بوحدة السنتيمترات.

```csharp
public double HeightCM { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyHeightCMDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف شكلاً مستطيلاً مع جميع المعلمات المطلوبة
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 100, 100);

            // تعيين الارتفاع بالسنتيمترات
            shape.HeightCM = 3;
            Console.WriteLine("Shape height: " + shape.HeightCM + " cm");

            // تعديل الارتفاع إذا كان 3 سم
            if (shape.HeightCM == 3)
            {
                shape.HeightCM = 1;
                Console.WriteLine("Modified shape height: " + shape.HeightCM + " cm");
            }
        }
    }
}
```

### انظر أيضًا

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


