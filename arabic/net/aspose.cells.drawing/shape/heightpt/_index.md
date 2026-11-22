---
title: "Shape.HeightPt"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Shape. تمثل ارتفاع الشكل بوحدة النقاط"
type: docs
url: /ar/net/aspose.cells.drawing/shape/heightpt/
---
## Shape.HeightPt property

يمثل ارتفاع الشكل، بوحدة النقاط.

```csharp
public double HeightPt { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyHeightPtDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف شكلًا نموذجيًا مع جميع المعلمات المطلوبة
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 50, 100);

            // تعيين والحصول على خاصية HeightPt
            shape.HeightPt = 50;
            Console.WriteLine("Shape height in points: " + shape.HeightPt);

            // تعديل الارتفاع إذا كان يطابق شرطًا
            if (shape.HeightPt == 50)
            {
                shape.HeightPt = 30;
                Console.WriteLine("Modified shape height: " + shape.HeightPt);
            }
        }
    }
}
```

### انظر أيضًا

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


