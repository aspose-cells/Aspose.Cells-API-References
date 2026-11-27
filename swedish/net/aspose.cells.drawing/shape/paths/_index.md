---
title: "Shape.Paths"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Shape-egenskap. Hämtar sökvägarna för en anpassad geometrisk form"
type: docs
url: /sv/net/aspose.cells.drawing/shape/paths/
---
## Shape.Paths property

Hämtar sökvägarna för en anpassad geometrisk form.

```csharp
public ShapePathCollection Paths { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyPathsDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en anpassad form (rektangel) med korrekta parametrar
            Shape shape = worksheet.Shapes.AddAutoShape(AutoShapeType.Rectangle, 1, 1, 1, 1, 100, 150);

            // Kontrollera om formen har anpassade geometriska sökvägar
            if (shape.Paths != null)
            {
                Console.WriteLine("Shape has custom geometry paths:");
                Console.WriteLine($"Number of paths: {shape.Paths.Count}");
                
                // Lägg till en ny sökväg till formens geometri
                int newPathIndex = shape.Paths.Add();
                Console.WriteLine($"Added new path at index: {newPathIndex}");
            }
            else
            {
                Console.WriteLine("No custom geometry path.");
            }
        }
    }
}
```

### Se även

* class [ShapePathCollection](../../shapepathcollection/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


