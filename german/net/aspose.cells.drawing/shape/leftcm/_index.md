---
title: "Shape.LeftCM"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Shape-Eigenschaft. Gibt den horizontalen Versatz der Form von ihrer linken Spalte in Zentimetern an"
type: docs
url: /de/net/aspose.cells.drawing/shape/leftcm/
---
## Shape.LeftCM property

Stellt den horizontalen Versatz der Form von ihrer linken Spalte dar, in der Einheit Zentimeter.

```csharp
public double LeftCM { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyLeftCMDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Rechteckform hinzufügen
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 100, 100);

            // LeftCM-Eigenschaft setzen und abrufen
            shape.LeftCM = 3.0;
            Console.WriteLine("Shape left position (cm): " + shape.LeftCM);

            // Linke Position ändern, wenn sie 3 cm beträgt
            if (shape.LeftCM == 3.0)
            {
                shape.LeftCM = 1.0;
                Console.WriteLine("Adjusted shape left position (cm): " + shape.LeftCM);
            }
        }
    }
}
```

### Siehe auch

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


