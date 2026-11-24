---
title: "Shape.IsFlippedHorizontally"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Shape-Eigenschaft. Liest und setzt, ob die Form horizontal gespiegelt ist"
type: docs
url: /de/net/aspose.cells.drawing/shape/isflippedhorizontally/
---
## Shape.IsFlippedHorizontally property

Liest und setzt, ob die Form horizontal gespiegelt ist.

```csharp
public bool IsFlippedHorizontally { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyIsFlippedHorizontallyDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispielhafte Form mit allen erforderlichen Parametern hinzufügen
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 0);

            // Prüfe und spiegle horizontal, wenn sie noch nicht gespiegelt ist
            if (shape.IsFlippedHorizontally == false)
            {
                shape.IsFlippedHorizontally = true;
                Console.WriteLine("Shape was flipped horizontally");
            }
            else
            {
                Console.WriteLine("Shape was already flipped horizontally");
            }
        }
    }
}
```

### Siehe auch

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


