---
title: "Shape.Spt"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية الشكل. تحدد رقمًا اختياريًا يمكن للتطبيق استخدامه لربط الشكل المحدد بنوع شكل معرف"
type: docs
url: /ar/net/aspose.cells.drawing/shape/spt/
---
## Shape.Spt property

يحدد رقمًا اختياريًا يمكن للتطبيق استخدامه لربط الشكل المحدد بنوع شكل معرف.

```csharp
public int Spt { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertySptDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف شكلًا مستطيلًا بالمعلمات الصحيحة
            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 1, 1, 100, 100, 100, 100);

            // احصل على خاصية Spt واعرضها
            int spt = shape.Spt;
            Console.WriteLine("Shape Spt value: " + spt);

            // أنشئ شكل بيضاوي جديد لتوضيح قيمة Spt المختلفة
            Shape ovalShape = worksheet.Shapes.AddShape(MsoDrawingType.Oval, 1, 1, 100, 100, 100, 100);
            Console.WriteLine("Oval shape Spt value: " + ovalShape.Spt);
        }
    }
}
```

### انظر أيضًا

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


