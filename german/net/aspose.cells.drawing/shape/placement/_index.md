---
title: "Shape.Placement"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Shape-Eigenschaft. Gibt an, wie das Zeichenobjekt an den darunter liegenden Zellen befestigt ist. Die Eigenschaft steuert die Platzierung eines Objekts auf einem Arbeitsblatt."
type: docs
url: /de/net/aspose.cells.drawing/shape/placement/
---
## Shape.Placement property

Stellt dar, wie das Zeichenobjekt an den darunter liegenden Zellen befestigt ist. Die Eigenschaft steuert die Platzierung eines Objekts auf einem Arbeitsblatt.

```csharp
public PlacementType Placement { get; set; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Eine Beispiel-Form hinzufügen
            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 200, 50);

            // Placement-Eigenschaft demonstrieren
            Console.WriteLine("Original Placement: " + shape.Placement);
            
            // Ändern Sie den Platzierungstyp.
            shape.Placement = PlacementType.MoveAndSize;
            Console.WriteLine("Modified Placement: " + shape.Placement);

            // Speichere die Arbeitsmappe
            workbook.Save("ShapePlacementDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [PlacementType](../../placementtype/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


