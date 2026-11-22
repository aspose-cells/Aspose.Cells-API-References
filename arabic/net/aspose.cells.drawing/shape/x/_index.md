---
title: "Shape.X"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Shape. تحصل وتضبط الإزاحة الأفقية للشكل من الحد الأيسر للورقة بوحدة البكسل"
type: docs
url: /ar/net/aspose.cells.drawing/shape/x/
---
## Shape.X property

يحصل ويضبط الإزاحة الأفقية للشكل من الحد الأيسر لورقة العمل، بوحدة البكسل.

```csharp
public int X { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyXDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة شكل مستطيل
            Shape shape = worksheet.Shapes.AddRectangle(10, 10, 100, 100, 0, 0);

            // عيّن الموضع الأولي X
            shape.X = 200;
            Console.WriteLine("Initial X position: " + shape.X);

            // عدّل موضع X إذا كان يساوي 3 (لتوضيح منطق حالة الاختبار)
            if (shape.X == 3)
            {
                shape.X = 1;
            }
            else
            {
                // للتوضيح، غيّر موضع X إلى 300
                shape.X = 300;
            }

            Console.WriteLine("Final X position: " + shape.X);
        }
    }
}
```

### انظر أيضًا

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


