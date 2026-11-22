---
title: "Shape.TopToCorner"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Shape. يحصل على ويضبط الإزاحة العمودية للشكل من الحد العلوي للورقة بوحدة البكسل"
type: docs
url: /ar/net/aspose.cells.drawing/shape/toptocorner/
---
## Shape.TopToCorner property

يحصل على ويضبط الإزاحة العمودية للشكل من الحد العلوي للورقة، بوحدة البكسل.

```csharp
public int TopToCorner { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyTopToCornerDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف شكلاً مستطيلًا إلى ورقة العمل
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 150, 0);

            // اضبط واعرض خاصية TopToCorner
            shape.TopToCorner = 50;
            Console.WriteLine("Shape TopToCorner: " + shape.TopToCorner);

            // عدّل خاصية TopToCorner
            if (shape.TopToCorner == 50)
            {
                shape.TopToCorner = 20;
                Console.WriteLine("Updated Shape TopToCorner: " + shape.TopToCorner);
            }
        }
    }
}
```

### انظر أيضًا

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


