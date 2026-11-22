---
title: "Shape.ToFrontOrBack"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Shape. يجلب الشكل إلى المقدمة أو يرسل الشكل إلى الخلف"
type: docs
url: /ar/net/aspose.cells.drawing/shape/tofrontorback/
---
## Shape.ToFrontOrBack method

ينقل الشكل إلى المقدمة أو يرسل الشكل إلى الخلف.

```csharp
public void ToFrontOrBack(int orders)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| ترتيبات | Int32 | إذا كان أقل من الصفر، يضع الشكل في الخلف. إذا كان أكبر من الصفر، يجلب الشكل إلى المقدمة. |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodToFrontOrBackWithInt32Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف شكلين لتوضيح ترتيب Z
            Aspose.Cells.Drawing.Shape shape1 = worksheet.Shapes.AddRectangle(10, 10, 100, 100, 0, 0);
            Aspose.Cells.Drawing.Shape shape2 = worksheet.Shapes.AddRectangle(50, 50, 100, 100, 0, 0);

            // حرك shape2 موقعين إلى الأمام في ترتيب Z
            shape2.ToFrontOrBack(2);

            // حرك shape1 موقعًا واحدًا إلى الخلف في ترتيب Z
            shape1.ToFrontOrBack(-1);
        }
    }
}
```

### انظر أيضًا

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


