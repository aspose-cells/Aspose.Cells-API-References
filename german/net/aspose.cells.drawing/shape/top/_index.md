---
title: "Shape.Top"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Shape-Eigenschaft. Stellt den vertikalen Versatz des Shapes von seiner oberen Zeile in Pixeln dar"
type: docs
url: /de/net/aspose.cells.drawing/shape/top/
---
## Shape.Top property

Stellt den vertikalen Versatz der Form von ihrer oberen Zeile dar, in Einheit Pixel.

```csharp
public int Top { get; set; }
```

### Hinweise

Wenn die Form im Diagramm ist, gibt sie den vertikalen Versatz der Form von ihrer oberen Begrenzung an.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyTopDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Rechteckform hinzufügen
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 100, 100);

            // Setzen Sie die anfängliche obere Position
            shape.Top = 50;
            Console.WriteLine("Initial Top position: " + shape.Top);

            // Ändern Sie die obere Position, wenn sie 3 ist (zur Demonstration der Testfalllogik)
            if (shape.Top == 3)
            {
                shape.Top = 1;
            }
            else
            {
                // Zur Demonstration setzen Sie sie auf 3 und wenden dann die Testfalllogik an
                shape.Top = 3;
                if (shape.Top == 3)
                {
                    shape.Top = 1;
                    Console.WriteLine("Modified Top position: " + shape.Top);
                }
            }
        }
    }
}
```

### Siehe auch

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


