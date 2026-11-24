---
title: "Shape.UpperLeftRow"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Shape-Eigenschaft. Repräsentiert den Index der oberen Zeile"
type: docs
url: /de/net/aspose.cells.drawing/shape/upperleftrow/
---
## Shape.UpperLeftRow property

Stellt den Index der obersten Zeile dar.

```csharp
public int UpperLeftRow { get; set; }
```

### Hinweise

Wenn die Form in der Form oder in der Gruppe ist, wird UpperLeftRow ignoriert.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyUpperLeftRowDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge dem Arbeitsblatt eine Form hinzu
            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 0, 0);

            // Setze und demonstriere die UpperLeftRow-Eigenschaft
            shape.UpperLeftRow = 3;
            Console.WriteLine("Shape's initial topRow: " + shape.UpperLeftRow);

            // Modifiziere UpperLeftRow basierend auf einer Bedingung
            if (shape.UpperLeftRow == 3)
                shape.UpperLeftRow = 1;

            Console.WriteLine("Shape's modified topRow: " + shape.UpperLeftRow);
        }
    }
}
```

### Siehe auch

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


