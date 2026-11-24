---
title: "Shape.HeightInch"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Shape-Eigenschaft. Gibt die Höhe der Form in Zoll an."
type: docs
url: /de/net/aspose.cells.drawing/shape/heightinch/
---
## Shape.HeightInch property

Stellt die Höhe der Form in Zoll dar.

```csharp
public double HeightInch { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyHeightInchDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge eine Rechteckform mit allen erforderlichen Parametern hinzu
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 100);

            // Setze und lese die Höhe in Zoll.
            shape.HeightInch = 3;
            Console.WriteLine("Shape height (inches): " + shape.HeightInch);

            // Ändere die Höhe, wenn die Bedingung erfüllt ist.
            if (shape.HeightInch == 3)
            {
                shape.HeightInch = 1;
                Console.WriteLine("Modified shape height (inches): " + shape.HeightInch);
            }
        }
    }
}
```

### Siehe auch

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


