---
title: "Shape.LowerDeltaY"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية الشكل. تحصل أو تعيّن الإزاحة الرأسية للشكل من صف زاويته السفلية اليمنى"
type: docs
url: /ar/net/aspose.cells.drawing/shape/lowerdeltay/
---
## Shape.LowerDeltaY property

يحصل أو يضبط الإزاحة العمودية للشكل من صف الزاوية السفلية اليمنى.

```csharp
public int LowerDeltaY { get; set; }
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
    public class ShapePropertyLowerDeltaYDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة شكل عينة مع المعلمات الصحيحة
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 100, 100);

            // تعيين وإظهار خاصية LowerDeltaY
            shape.LowerDeltaY = 20;
            Console.WriteLine("Initial LowerDeltaY: " + shape.LowerDeltaY);

            // تعديل LowerDeltaY بشكل شرطي
            if (shape.LowerDeltaY == 20)
            {
                shape.LowerDeltaY = 10;
                Console.WriteLine("Modified LowerDeltaY: " + shape.LowerDeltaY);
            }
        }
    }
}
```

### انظر أيضًا

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


