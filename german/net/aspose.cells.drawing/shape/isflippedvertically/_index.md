---
title: "Shape.IsFlippedVertically"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Shape-Eigenschaft. Ermittelt und legt fest, ob das Shape vertikal gespiegelt ist."
type: docs
url: /de/net/aspose.cells.drawing/shape/isflippedvertically/
---
## Shape.IsFlippedVertically property

Ermittelt und setzt, ob die Form vertikal gespiegelt ist .

```csharp
public bool IsFlippedVertically { get; set; }
```

### Beispiele

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

### Siehe auch

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


