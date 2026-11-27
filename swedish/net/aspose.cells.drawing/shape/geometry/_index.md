---
title: "Shape.Geometry"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Shape-egenskap. Hämtar geometrin"
type: docs
url: /sv/net/aspose.cells.drawing/shape/geometry/
---
## Shape.Geometry property

Hämtar geometrin

```csharp
public Geometry Geometry { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyGeometryDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en rektangelform med korrekta parametrar
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 0);

            // Kontrollera geometriegenskaper
            if (shape.Geometry != null)
            {
                Console.WriteLine("Shape has geometry path with " + shape.Geometry.ShapeAdjustValues.Count + " adjustment points");
                
                // Lägg till en justeringspunkt (demonstrerar geometrimodifiering)
                shape.Geometry.ShapeAdjustValues.Add("adj1", 0.5);
                Console.WriteLine("Added adjustment point. Total now: " + shape.Geometry.ShapeAdjustValues.Count);
            }

            // Spara arbetsboken
            workbook.Save("ShapeGeometryDemo.xlsx");
        }
    }
}
```

### Se även

* class [Geometry](../../geometry/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


