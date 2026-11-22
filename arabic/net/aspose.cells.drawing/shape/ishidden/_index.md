---
title: "Shape.IsHidden"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية الشكل. تشير إلى ما إذا كان الكائن مرئيًا"
type: docs
url: /ar/net/aspose.cells.drawing/shape/ishidden/
---
## Shape.IsHidden property

يشير إلى ما إذا كان الكائن مرئياً.

```csharp
public bool IsHidden { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyIsHiddenDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة شكل إلى ورقة العمل
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 0);

            // تعيين خاصية IsHidden إلى false (مرئي)
            shape.IsHidden = false;
            Console.WriteLine("Shape is visible: " + !shape.IsHidden);

            // تعيين خاصية IsHidden إلى true (مخفي)
            shape.IsHidden = true;
            Console.WriteLine("Shape is hidden: " + shape.IsHidden);
        }
    }
}
```

### انظر أيضًا

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


