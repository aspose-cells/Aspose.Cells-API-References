---
title: "Shape.Left"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Shape. تمثل الإزاحة الأفقية للشكل من العمود الأيسر بوحدة البكسل"
type: docs
url: /ar/net/aspose.cells.drawing/shape/left/
---
## Shape.Left property

يمثل الإزاحة الأفقية للشكل من عموده الأيسر، بوحدة البكسل.

```csharp
public int Left { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyLeftDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة شكل لعرض خاصية Left
            Shape shape = worksheet.Shapes.AddRectangle(10, 10, 100, 100, 0, 0);

            // تعيين الموضع الأيسر الأولي
            shape.Left = 200;
            Console.WriteLine("Shape Left position: " + shape.Left);

            // تعديل موضع Left بشكل شرطي
            if (shape.Left == 200)
            {
                shape.Left = 150;
                Console.WriteLine("Adjusted Shape Left position: " + shape.Left);
            }
        }
    }
}
```

### انظر أيضًا

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


