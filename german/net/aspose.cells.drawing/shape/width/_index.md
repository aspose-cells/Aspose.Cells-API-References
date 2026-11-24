---
title: "Shape.Width"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Shape-Eigenschaft. Stellt die Breite der Form in Pixeln dar"
type: docs
url: /de/net/aspose.cells.drawing/shape/width/
---
## Shape.Width property

Stellt die Breite der Form in Pixeln dar.

```csharp
public int Width { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyWidthDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge ein Rechteck shape mit korrekten Parametern hinzu
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 50);

            // Setze die Anfangsbreite und zeige sie an
            shape.Width = 300;
            Console.WriteLine("Initial width: " + shape.Width);

            // Breite basierend auf einer Bedingung ändern
            if (shape.Width == 300)
                shape.Width = 150;

            Console.WriteLine("Modified width: " + shape.Width);
        }
    }
}
```

### Siehe auch

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


