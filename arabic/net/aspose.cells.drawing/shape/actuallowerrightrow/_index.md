---
title: "Shape.ActualLowerRightRow"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Shape. احصل على الصف السفلي الفعلي"
type: docs
url: /ar/net/aspose.cells.drawing/shape/actuallowerrightrow/
---
## Shape.ActualLowerRightRow property

احصل على الصف السفلي الفعلي.

```csharp
public int ActualLowerRightRow { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyActualLowerRightRowDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف شكلًا نموذجيًا (مستطيل)
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 150, 100);

            // احصل على الصف السفلي الأيمن الفعلي للشكل
            int actualLowerRightRow = shape.ActualLowerRightRow;

            // أخرج النتيجة.
            Console.WriteLine("Actual Lower Right Row of the shape: " + actualLowerRightRow);
        }
    }
}
```

### انظر أيضًا

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


