---
title: "Shape.Placement"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Shape. تمثل الطريقة التي يتم بها إرفاق كائن الرسم بالخلايا أسفله. تتحكم الخاصية في وضع الكائن على ورقة العمل"
type: docs
url: /ar/net/aspose.cells.drawing/shape/placement/
---
## Shape.Placement property

يمثل الطريقة التي يتم بها إرفاق كائن الرسم بالخلايا تحته. تتحكم الخاصية في وضع الكائن على ورقة العمل.

```csharp
public PlacementType Placement { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyPlacementDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف شكلًا تجريبيًا
            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 200, 50);

            // عرض خاصية Placement
            Console.WriteLine("Original Placement: " + shape.Placement);
            
            // غيّر نوع الوضع
            shape.Placement = PlacementType.MoveAndSize;
            Console.WriteLine("Modified Placement: " + shape.Placement);

            // احفظ المصنف
            workbook.Save("ShapePlacementDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [PlacementType](../../placementtype/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


