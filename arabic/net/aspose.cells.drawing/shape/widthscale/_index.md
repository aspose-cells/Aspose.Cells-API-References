---
title: "Shape.WidthScale"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Shape. تحصل وتضبط مقياس العرض بوحدة النسبة المئوية لعرض الصورة الأصلية. إذا لم يكن الشكل صورة، فإن خاصية WidthScale تُعيد فقط 100"
type: docs
url: /ar/net/aspose.cells.drawing/shape/widthscale/
---
## Shape.WidthScale property

يحصل أو يضبط مقياس العرض بوحدة النسبة المئوية لعرض الصورة الأصلية. إذا لم يكن الشكل صورة، فإن خاصية WidthScale تُعيد دائمًا 100؛

```csharp
public int WidthScale { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyWidthScaleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف شكلًا مستطيلًا بالمعلمات الصحيحة
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 0);

            // اضبط مقياس العرض الأولي
            shape.WidthScale = 50;
            Console.WriteLine("Initial WidthScale: " + shape.WidthScale);

            // عدّل مقياس العرض إذا تم استيفاء الشرط
            if (shape.WidthScale == 50)
            {
                shape.WidthScale = 75;
                Console.WriteLine("Updated WidthScale: " + shape.WidthScale);
            }

            // احفظ المصنف
            workbook.Save("ShapeWidthScaleDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


