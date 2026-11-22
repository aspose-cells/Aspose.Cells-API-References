---
title: "Shape.Fill"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Shape. تُرجع كائن FillFormat يحتوي على خصائص تنسيق التعبئة للشكل المحدد"
type: docs
url: /ar/net/aspose.cells.drawing/shape/fill/
---
## Shape.Fill property

إرجاع كائن [`FillFormat`](../fillformat/) يحتوي على خصائص تنسيق التعبئة للشكل المحدد.

```csharp
public FillFormat Fill { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyFillDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف شكلًا مستطيلًا بالمعلمات الصحيحة
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 0);

            // احصل على تنسيق الملء للشكل
            FillFormat fillFmt = shape.Fill;

            // تعيين ملء صلب باللون
            fillFmt.SolidFill.Color = System.Drawing.Color.Red;

            // ضبط الشفافية
            fillFmt.Transparency = 0.5;

            // احفظ المصنف
            workbook.Save("ShapeFillDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [FillFormat](../../fillformat/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


