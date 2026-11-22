---
title: "Shape.HeightScale"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Shape. تحصل وتضبط مقياس الارتفاع بوحدة النسبة المئوية لارتفاع الصورة الأصلية. إذا لم يكن الشكل صورة فإن خاصية HeightScale تعيد 100 فقط"
type: docs
url: /ar/net/aspose.cells.drawing/shape/heightscale/
---
## Shape.HeightScale property

يحصل أو يحدد مقياس الارتفاع، بوحدة النسبة المئوية لارتفاع الصورة الأصلية. إذا لم يكن الشكل صورة، فإن خاصية HeightScale تُعيد فقط 100؛

```csharp
public int HeightScale { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyHeightScaleDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة شكل مستطيل
            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 200, 150);

            // تعيين مقياس الارتفاع الأولي
            shape.HeightScale = 50;
            Console.WriteLine("Initial HeightScale: " + shape.HeightScale);

            // تعديل مقياس الارتفاع إذا تم استيفاء الشرط
            if (shape.HeightScale == 50)
            {
                shape.HeightScale = 75;
                Console.WriteLine("Modified HeightScale: " + shape.HeightScale);
            }
        }
    }
}
```

### انظر أيضًا

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


