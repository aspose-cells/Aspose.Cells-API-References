---
title: "Shape.LeftInch"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Shape-Eigenschaft. Gibt den horizontalen Versatz der Form von ihrer linken Spalte in Zoll an."
type: docs
url: /de/net/aspose.cells.drawing/shape/leftinch/
---
## Shape.LeftInch property

Stellt den horizontalen Versatz der Form von ihrer linken Spalte dar, in der Einheit Zoll.

```csharp
public double LeftInch { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyLeftInchDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispielhafte Form mit allen erforderlichen Parametern hinzufügen
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 100, 100);

            // LeftInch-Eigenschaft festlegen und demonstrieren
            shape.LeftInch = 3;
            Console.WriteLine("Shape left position (inches): " + shape.LeftInch);

            // Linke Position ändern, wenn sie 3 Zoll beträgt
            if (shape.LeftInch == 3)
            {
                shape.LeftInch = 1;
                Console.WriteLine("Adjusted shape left position (inches): " + shape.LeftInch);
            }
        }
    }
}
```

### Siehe auch

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


