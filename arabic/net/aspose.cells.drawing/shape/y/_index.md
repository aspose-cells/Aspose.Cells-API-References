---
title: "Shape.Y"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Shape. تحصل وتضبط الإزاحة العمودية للشكل من الحد العلوي للورقة بوحدة البكسل"
type: docs
url: /ar/net/aspose.cells.drawing/shape/y/
---
## Shape.Y property

يحصل أو يضبط الإزاحة العمودية للشكل من الحد العلوي لورقة العمل، بوحدة البكسل.

```csharp
public int Y { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyYDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة شكل مستطيل
            Aspose.Cells.Drawing.Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 0, 0);

            // قم بتعيين وإظهار خاصية Y
            shape.Y = 200;
            Console.WriteLine("Shape Y position: " + shape.Y);

            // عدّل موضع Y بناءً على الشرط
            if (shape.Y == 200)
                shape.Y = 100;

            Console.WriteLine("Updated Shape Y position: " + shape.Y);
        }
    }
}
```

### انظر أيضًا

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


