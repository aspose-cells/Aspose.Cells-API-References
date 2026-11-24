---
title: "Shape.WidthScale"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Shape-Eigenschaft. Gibt den Breitenmaßstab in Prozent der ursprünglichen Bildbreite zurück und legt ihn fest. Wenn die Form kein Bild ist, gibt die WidthScale‑Eigenschaft nur 100 zurück"
type: docs
url: /de/net/aspose.cells.drawing/shape/widthscale/
---
## Shape.WidthScale property

Liest und setzt die Breiten­skalierung in Prozent der ursprünglichen Bildbreite. Wenn die Form kein Bild ist, gibt die WidthScale‑Eigenschaft nur 100 zurück;

```csharp
public int WidthScale { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyWidthScaleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge ein Rechteck shape mit korrekten Parametern hinzu
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 0);

            // Initialen Breitenmaßstab festlegen
            shape.WidthScale = 50;
            Console.WriteLine("Initial WidthScale: " + shape.WidthScale);

            // Breitenmaßstab ändern, wenn die Bedingung erfüllt ist
            if (shape.WidthScale == 50)
            {
                shape.WidthScale = 75;
                Console.WriteLine("Updated WidthScale: " + shape.WidthScale);
            }

            // Speichere die Arbeitsmappe
            workbook.Save("ShapeWidthScaleDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


