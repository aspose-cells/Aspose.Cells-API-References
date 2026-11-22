---
title: "Shape.GetConnectionPoints"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Shape. الحصول على نقاط الاتصال"
type: docs
url: /ar/net/aspose.cells.drawing/shape/getconnectionpoints/
---
## Shape.GetConnectionPoints method

احصل على نقاط الاتصال

```csharp
public float[][] GetConnectionPoints()
```

### قيمة الإرجاع

[X,Y] pairs of the connection point. Every item is a float[2] array, [0] represents x and [1] represents y.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodGetConnectionPointsDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف شكلاً إلى ورقة العمل مع جميع المعلمات المطلوبة
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 0);

            // الحصول على نقاط الاتصال للشكل
            float[][] points = shape.GetConnectionPoints();

            // إخراج نقاط الاتصال
            Console.WriteLine("Connection Points:");
            for (int i = 0; i < points.Length; i++)
            {
                Console.WriteLine($"Point {i + 1}: X={points[i][0]}, Y={points[i][1]}");
            }
        }
    }
}
```

### انظر أيضًا

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


