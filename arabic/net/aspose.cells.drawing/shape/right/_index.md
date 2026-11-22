---
title: "Shape.Right"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Shape. تمثل عرض الإزاحة الأفقية للشكل من عمود الزاوية السفلية اليمنى بوحدة البكسل"
type: docs
url: /ar/net/aspose.cells.drawing/shape/right/
---
## Shape.Right property

يمثل عرض الإزاحة الأفقية للشكل من عمود الزاوية السفلية اليمنى، بوحدة البكسل.

```csharp
public int Right { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyRightDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة شكل إلى ورقة العمل
            Aspose.Cells.Drawing.Shape shape = worksheet.Shapes.AddRectangle(10, 10, 100, 100, 0, 0);

            // اضبط واحصل على خاصية Right
            shape.Right = 200;
            Console.WriteLine("Shape Right position: " + shape.Right);

            // عدّل خاصية Right شرطياً
            if (shape.Right == 200)
                shape.Right = 150;

            Console.WriteLine("Modified Shape Right position: " + shape.Right);
        }
    }
}
```

### انظر أيضًا

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


