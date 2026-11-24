---
title: "Shape.HeightPt"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Shape-Eigenschaft. Stellt die Höhe der Form in Punkt als Einheit dar"
type: docs
url: /de/net/aspose.cells.drawing/shape/heightpt/
---
## Shape.HeightPt property

Stellt die Höhe der Form in Punkten dar.

```csharp
public double HeightPt { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyHeightPtDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispielhafte Form mit allen erforderlichen Parametern hinzufügen
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 50, 100);

            // HeightPt-Eigenschaft festlegen und abrufen
            shape.HeightPt = 50;
            Console.WriteLine("Shape height in points: " + shape.HeightPt);

            // Höhe ändern, wenn sie einer Bedingung entspricht
            if (shape.HeightPt == 50)
            {
                shape.HeightPt = 30;
                Console.WriteLine("Modified shape height: " + shape.HeightPt);
            }
        }
    }
}
```

### Siehe auch

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


