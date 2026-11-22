---
title: "Shape.ZOrderPosition"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Shape. تُرجع موضع الشكل في ترتيب ZOrder"
type: docs
url: /ar/net/aspose.cells.drawing/shape/zorderposition/
---
## Shape.ZOrderPosition property

إرجاع موضع الشكل في ترتيب z.

```csharp
public int ZOrderPosition { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyZOrderPositionDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة ثلاثة أشكال لعرض ZOrder
            Shape shape1 = worksheet.Shapes.AddRectangle(10, 10, 100, 100, 0, 0);
            Shape shape2 = worksheet.Shapes.AddRectangle(50, 50, 100, 100, 0, 0);
            Shape shape3 = worksheet.Shapes.AddRectangle(90, 90, 100, 100, 0, 0);

            // تعيين مواضع ZOrder
            shape1.ZOrderPosition = 0;
            shape2.ZOrderPosition = 1;
            shape3.ZOrderPosition = 2;

            // تغيير ZOrder للـ shape3 لجعله في المقدمة
            shape3.ZOrderPosition = 0;

            // احفظ المصنف
            workbook.Save("ShapeZOrderDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


