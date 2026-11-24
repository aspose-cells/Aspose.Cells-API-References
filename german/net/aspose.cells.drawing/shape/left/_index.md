---
title: "Shape.Left"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Shape-Eigenschaft. Stellt den horizontalen Abstand der Form von ihrer linken Spalte in Pixeln dar"
type: docs
url: /de/net/aspose.cells.drawing/shape/left/
---
## Shape.Left property

Stellt den horizontalen Versatz der Form von ihrer linken Spalte dar, in der Einheit Pixel.

```csharp
public int Left { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyLeftDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge eine Form hinzu, um die Left-Eigenschaft zu demonstrieren
            Shape shape = worksheet.Shapes.AddRectangle(10, 10, 100, 100, 0, 0);

            // Setze die anfängliche Left-Position
            shape.Left = 200;
            Console.WriteLine("Shape Left position: " + shape.Left);

            // Left-Position bedingt ändern
            if (shape.Left == 200)
            {
                shape.Left = 150;
                Console.WriteLine("Adjusted Shape Left position: " + shape.Left);
            }
        }
    }
}
```

### Siehe auch

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


