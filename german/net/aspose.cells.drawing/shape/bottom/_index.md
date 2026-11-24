---
title: "Shape.Bottom"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Shape-Eigenschaft. Gibt die Breite des vertikalen Versatzes der Form von ihrer unteren Ecke in Pixeln an"
type: docs
url: /de/net/aspose.cells.drawing/shape/bottom/
---
## Shape.Bottom property

Stellt die Breite des vertikalen Versatzes der Form von ihrer unteren Eckzeilenposition dar, in Pixeln.

```csharp
public int Bottom { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyBottomDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispielhafte Form mit allen erforderlichen Parametern hinzufügen
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 100, 100);

            // Anfangsposition festlegen
            shape.Top = 200;
            shape.Left = 200;

            // Bottom-Eigenschaft demonstrieren
            Console.WriteLine("Original Bottom position: " + shape.Bottom);

            // Bottom-Position ändern
            if (shape.Bottom == 300)  // 200 (Top) + 100 (Height)
            {
                shape.Bottom = 250;  // This will change the Top position (250 - 100 = 150)
                Console.WriteLine("New Bottom position: " + shape.Bottom);
                Console.WriteLine("New Top position: " + shape.Top);
            }
        }
    }
}
```

### Siehe auch

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


