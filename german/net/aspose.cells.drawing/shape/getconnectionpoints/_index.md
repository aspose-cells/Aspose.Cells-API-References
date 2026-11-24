---
title: "Shape.GetConnectionPoints"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Shape-Methode. Gibt die Verbindungspunkte zurück"
type: docs
url: /de/net/aspose.cells.drawing/shape/getconnectionpoints/
---
## Shape.GetConnectionPoints method

Lese die Verbindungspunkte

```csharp
public float[][] GetConnectionPoints()
```

### Rückgabewert

[X,Y] pairs of the connection point. Every item is a float[2] array, [0] represents x and [1] represents y.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodGetConnectionPointsDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügt dem Arbeitsblatt eine Form mit allen erforderlichen Parametern hinzu
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 0);

            // Verbindungspunkte der Form abrufen
            float[][] points = shape.GetConnectionPoints();

            // Gib die Verbindungspunkte aus
            Console.WriteLine("Connection Points:");
            for (int i = 0; i < points.Length; i++)
            {
                Console.WriteLine($"Point {i + 1}: X={points[i][0]}, Y={points[i][1]}");
            }
        }
    }
}
```

### Siehe auch

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


