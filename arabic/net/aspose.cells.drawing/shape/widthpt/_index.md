---
title: "Shape.WidthPt"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Shape. تمثّل عرض الشكل بوحدة النقطة"
type: docs
url: /ar/net/aspose.cells.drawing/shape/widthpt/
---
## Shape.WidthPt property

يمثل عرض الشكل بوحدة النقطة.

```csharp
public double WidthPt { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyWidthPtDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة شكل مستطيل
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 0);

            // عيّن واحصل على العرض بالنقاط
            shape.WidthPt = 150;
            Console.WriteLine("Shape width in points: " + shape.WidthPt);

            // تعديل العرض إذا تم استيفاء الشرط
            if (shape.WidthPt == 150)
            {
                shape.WidthPt = 100;
                Console.WriteLine("Modified shape width in points: " + shape.WidthPt);
            }
        }
    }
}
```

### انظر أيضًا

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


