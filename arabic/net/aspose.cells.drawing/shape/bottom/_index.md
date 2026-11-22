---
title: "Shape.Bottom"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Shape. تمثل عرض الإزاحة العمودية للشكل من صف زاوية القاع السفلية بوحدة البكسل"
type: docs
url: /ar/net/aspose.cells.drawing/shape/bottom/
---
## Shape.Bottom property

يمثل عرض الإزاحة العمودية للشكل من صف الزاوية السفلية، بوحدة البكسل.

```csharp
public int Bottom { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyBottomDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف شكلًا نموذجيًا مع جميع المعلمات المطلوبة
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 100, 100);

            // تعيين الموضع الأولي
            shape.Top = 200;
            shape.Left = 200;

            // عرض خاصية Bottom
            Console.WriteLine("Original Bottom position: " + shape.Bottom);

            // تعديل موضع Bottom
            if (shape.Bottom == 300)  // 200 (Top) + 100 (Height)
            {
                shape.Bottom = 250;  // This will change the Top position (250 - 100 = 150)
                Console.WriteLine("New Bottom position: " + shape.Bottom);
                Console.WriteLine("New Top position: " + shape.Top);
            }
        }
    }
}
```

### انظر أيضًا

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


