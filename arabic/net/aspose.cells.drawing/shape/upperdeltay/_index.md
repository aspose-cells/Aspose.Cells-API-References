---
title: "Shape.UpperDeltaY"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Shape. تحصل أو تعين الإزاحة العمودية للشكل من صف الزاوية العلوية اليسرى."
type: docs
url: /ar/net/aspose.cells.drawing/shape/upperdeltay/
---
## Shape.UpperDeltaY property

يحصل أو يضبط الإزاحة العمودية للشكل من صف الزاوية العلوية اليسرى.

```csharp
public int UpperDeltaY { get; set; }
```

### ملاحظات

نطاق القيمة هو من 0 إلى 256.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyUpperDeltaYDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف شكلاً لتوضيح خاصية UpperDeltaY
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 100, 100);

            // تعيين وعرض قيمة UpperDeltaY الأولية
            shape.UpperDeltaY = 3;
            Console.WriteLine("Initial UpperDeltaY: " + shape.UpperDeltaY);

            // تعديل قيمة UpperDeltaY
            if (shape.UpperDeltaY == 3)
            {
                shape.UpperDeltaY = 1;
                Console.WriteLine("Modified UpperDeltaY: " + shape.UpperDeltaY);
            }
        }
    }
}
```

### انظر أيضًا

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


