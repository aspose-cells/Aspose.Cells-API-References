---
title: "Shape.IsFlippedVertically"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Shape. تحصل وتعيّن ما إذا كان الشكل مقلوبًا عموديًا"
type: docs
url: /ar/net/aspose.cells.drawing/shape/isflippedvertically/
---
## Shape.IsFlippedVertically property

يحصل أو يحدد ما إذا كان الشكل مقلوبًا عموديًا.

```csharp
public bool IsFlippedVertically { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyIsFlippedVerticallyDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 0);
            
            Console.WriteLine("Original IsFlippedVertically: " + shape.IsFlippedVertically);
            
            if (shape.IsFlippedVertically == false)
            {
                shape.IsFlippedVertically = true;
                Console.WriteLine("Shape has been flipped vertically");
            }
            
            Console.WriteLine("Current IsFlippedVertically: " + shape.IsFlippedVertically);
        }
    }
}
```

### انظر أيضًا

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


