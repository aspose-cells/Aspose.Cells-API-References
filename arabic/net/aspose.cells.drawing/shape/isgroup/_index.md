---
title: "Shape.IsGroup"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Shape. تشير إلى ما إذا كان هذا الشكل شكل مجموعة"
type: docs
url: /ar/net/aspose.cells.drawing/shape/isgroup/
---
## Shape.IsGroup property

يشير إلى ما إذا كان هذا الشكل مجموعة أشكال.

```csharp
public bool IsGroup { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyIsGroupDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Shape shape1 = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 100, 100);
            Shape shape2 = worksheet.Shapes.AddRectangle(0, 100, 0, 100, 100, 100);
            Shape[] shapesToGroup = { shape1, shape2 };
            worksheet.Shapes.Group(shapesToGroup);

            Shape shape3 = worksheet.Shapes.AddOval(0, 200, 0, 200, 100, 100);

            for (int i = 0; i < worksheet.Shapes.Count; i++)
            {
                Shape shape = worksheet.Shapes[i];
                if (shape.IsGroup)
                {
                    Console.WriteLine("Group shape found at index: " + i);
                }
            }
        }
    }
}
```

### انظر أيضًا

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


