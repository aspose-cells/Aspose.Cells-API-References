---
title: "Shape.HeightScale"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Shape-Eigenschaft. Gibt den Höhenmaßstab in Prozent der ursprünglichen Bildhöhe zurück und setzt ihn. Wenn die Form kein Bild ist, gibt die HeightScale-Eigenschaft nur 100 zurück."
type: docs
url: /de/net/aspose.cells.drawing/shape/heightscale/
---
## Shape.HeightScale property

Ermittelt und setzt die Höhenskalierung, in Prozent der ursprünglichen Bildhöhe. Wenn die Form kein Bild ist, gibt die HeightScale‑Eigenschaft nur 100 zurück;

```csharp
public int HeightScale { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyHeightScaleDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Rechteckform hinzufügen
            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 200, 150);

            // Anfangs-Höhenmaßstab festlegen
            shape.HeightScale = 50;
            Console.WriteLine("Initial HeightScale: " + shape.HeightScale);

            // Höhenmaßstab ändern, wenn die Bedingung erfüllt ist
            if (shape.HeightScale == 50)
            {
                shape.HeightScale = 75;
                Console.WriteLine("Modified HeightScale: " + shape.HeightScale);
            }
        }
    }
}
```

### Siehe auch

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


