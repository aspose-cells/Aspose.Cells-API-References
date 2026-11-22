---
title: "Shape.IsAspectRatioLocked"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Shape. True يعني أن نسبة الأبعاد للشكل مقفلة"
type: docs
url: /ar/net/aspose.cells.drawing/shape/isaspectratiolocked/
---
## Shape.IsAspectRatioLocked property

True يعني أن نسبة أبعاد الشكل مقفلة.

```csharp
public bool IsAspectRatioLocked { get; set; }
```

### ملاحظات

فقط للصور وكائنات Ole.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyIsAspectRatioLockedDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 50);
            
            Console.WriteLine("Original Aspect Ratio Locked: " + shape.IsAspectRatioLocked);
            
            shape.IsAspectRatioLocked = true;
            Console.WriteLine("After setting to true: " + shape.IsAspectRatioLocked);
            
            shape.IsAspectRatioLocked = false;
            Console.WriteLine("After setting to false: " + shape.IsAspectRatioLocked);
        }
    }
}
```

### انظر أيضًا

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


