---
title: "Shape.GetConnectionPoints"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Shape-metod. Hämta anslutningspunkterna"
type: docs
url: /sv/net/aspose.cells.drawing/shape/getconnectionpoints/
---
## Shape.GetConnectionPoints method

Hämta anslutningspunkterna

```csharp
public float[][] GetConnectionPoints()
```

### Returvärde

[X,Y] pairs of the connection point. Every item is a float[2] array, [0] represents x and [1] represents y.

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en form i kalkylbladet med alla nödvändiga parametrar
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 0);

            // Hämta anslutningspunkterna för formen
            float[][] points = shape.GetConnectionPoints();

            // Skriv ut anslutningspunkterna
            Console.WriteLine("Connection Points:");
            for (int i = 0; i < points.Length; i++)
            {
                Console.WriteLine($"Point {i + 1}: X={points[i][0]}, Y={points[i][1]}");
            }
        }
    }
}
```

### Se även

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


