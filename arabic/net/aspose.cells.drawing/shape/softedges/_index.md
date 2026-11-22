---
title: "Shape.SoftEdges"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية الشكل. تحصل وتعيّن نصف قطر الضبابية لتطبيقه على الحواف بوحدة النقاط"
type: docs
url: /ar/net/aspose.cells.drawing/shape/softedges/
---
## Shape.SoftEdges property

الحصول على وتعيين نصف قطر الضبابية لتطبيقه على الحواف، بوحدة النقاط.

```csharp
public double SoftEdges { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertySoftEdgesDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف شكلًا مستطيلًا بالمعلمات الصحيحة
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 0);

            // تعيين تأثير الحواف الناعمة بنصف قطر 5 نقاط (0.5d = 5 نقاط)
            shape.SoftEdges = 0.5d;

            // احفظ المصنف
            workbook.Save("SoftEdgesDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


