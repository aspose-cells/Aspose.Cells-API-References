---
title: "Shape.LeftToCorner"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Shape-Eigenschaft. Gibt den horizontalen Versatz des Shapes vom linken Tabellenrand zurück und legt ihn fest"
type: docs
url: /de/net/aspose.cells.drawing/shape/lefttocorner/
---
## Shape.LeftToCorner property

Liest und setzt den horizontalen Versatz der Form vom linken Rand des Arbeitsblatts.

```csharp
public int LeftToCorner { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyLeftToCornerDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge ein Rechteck shape mit korrekten Parametern hinzu
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 150, 0);

            // Setzen und demonstrieren Sie die LeftToCorner-Eigenschaft
            shape.LeftToCorner = 50;
            Console.WriteLine("Shape LeftToCorner value: " + shape.LeftToCorner);

            // Ändern Sie LeftToCorner, wenn es einem bestimmten Wert entspricht
            if (shape.LeftToCorner == 50)
            {
                shape.LeftToCorner = 30;
                Console.WriteLine("Modified LeftToCorner value: " + shape.LeftToCorner);
            }
        }
    }
}
```

### Siehe auch

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


