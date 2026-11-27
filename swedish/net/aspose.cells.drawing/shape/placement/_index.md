---
title: "Shape.Placement"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Shape‑egenskap. Representerar hur ritobjektet är fäst vid cellerna under det. Egenskapen styr placeringen av ett objekt i ett kalkylblad."
type: docs
url: /sv/net/aspose.cells.drawing/shape/placement/
---
## Shape.Placement property

Representerar hur ritningsobjektet är fäst vid cellerna under det. Egenskapen styr placeringen av ett objekt på ett arbetsblad.

```csharp
public PlacementType Placement { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyPlacementDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en exempelform
            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 200, 50);

            // Demonstrera Placement‑egenskapen
            Console.WriteLine("Original Placement: " + shape.Placement);
            
            // Ändra placeringstyp
            shape.Placement = PlacementType.MoveAndSize;
            Console.WriteLine("Modified Placement: " + shape.Placement);

            // Spara arbetsboken
            workbook.Save("ShapePlacementDemo.xlsx");
        }
    }
}
```

### Se även

* enum [PlacementType](../../placementtype/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


