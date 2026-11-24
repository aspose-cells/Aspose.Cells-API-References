---
title: "Shape.Geometry"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Shape-Eigenschaft. Ruft die Geometrie ab."
type: docs
url: /de/net/aspose.cells.drawing/shape/geometry/
---
## Shape.Geometry property

Liest die Geometrie

```csharp
public Geometry Geometry { get; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge ein Rechteck shape mit korrekten Parametern hinzu
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 0);

            // Geometrieeigenschaften prüfen.
            if (shape.Geometry != null)
            {
                Console.WriteLine("Shape has geometry path with " + shape.Geometry.ShapeAdjustValues.Count + " adjustment points");
                
                // Fügen Sie einen Anpassungspunkt hinzu (zeigt die Geometrieänderung).
                shape.Geometry.ShapeAdjustValues.Add("adj1", 0.5);
                Console.WriteLine("Added adjustment point. Total now: " + shape.Geometry.ShapeAdjustValues.Count);
            }

            // Speichere die Arbeitsmappe
            workbook.Save("ShapeGeometryDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Geometry](../../geometry/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


