---
title: "Shape.LeftToCorner"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Shape. يحصل على ويضبط الإزاحة الأفقية للشكل من الحد الأيسر للورقة"
type: docs
url: /ar/net/aspose.cells.drawing/shape/lefttocorner/
---
## Shape.LeftToCorner property

يحصل على ويضبط الإزاحة الأفقية للشكل من الحد الأيسر للورقة.

```csharp
public int LeftToCorner { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyLeftToCornerDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف شكلًا مستطيلًا بالمعلمات الصحيحة
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 150, 0);

            // اضبط ووضح خاصية LeftToCorner
            shape.LeftToCorner = 50;
            Console.WriteLine("Shape LeftToCorner value: " + shape.LeftToCorner);

            // عدّل LeftToCorner إذا كان يساوي قيمة معينة
            if (shape.LeftToCorner == 50)
            {
                shape.LeftToCorner = 30;
                Console.WriteLine("Modified LeftToCorner value: " + shape.LeftToCorner);
            }
        }
    }
}
```

### انظر أيضًا

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


