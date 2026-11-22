---
title: "Shape.LowerRightRow"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Shape. تمثل فهرس الصف للزاوية السفلية اليمنى"
type: docs
url: /ar/net/aspose.cells.drawing/shape/lowerrightrow/
---
## Shape.LowerRightRow property

يمثل فهرس الصف للزاوية السفلية اليمنى.

```csharp
public int LowerRightRow { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyLowerRightRowDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة شكل إلى ورقة العمل
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 100, 100);

            // تعيين وإظهار خاصية LowerRightRow
            Console.WriteLine("Original LowerRightRow: " + shape.LowerRightRow);
            shape.LowerRightRow = 3;
            Console.WriteLine("Modified LowerRightRow: " + shape.LowerRightRow);

            // تعديل شرطي وفقًا لحالة الاختبار
            if (shape.LowerRightRow == 3)
            {
                shape.LowerRightRow = 1;
                Console.WriteLine("Final LowerRightRow after condition: " + shape.LowerRightRow);
            }
        }
    }
}
```

### انظر أيضًا

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


