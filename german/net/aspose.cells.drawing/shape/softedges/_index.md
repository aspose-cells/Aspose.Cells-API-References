---
title: "Shape.SoftEdges"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Shape-Eigenschaft. Gibt den Radius der Unschärfe zurück und legt ihn fest, der auf die Kanten in Punkten angewendet wird"
type: docs
url: /de/net/aspose.cells.drawing/shape/softedges/
---
## Shape.SoftEdges property

Liest und setzt den Radius der Unschärfe, die auf die Kanten angewendet wird, in Punkt-Einheiten.

```csharp
public double SoftEdges { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertySoftEdgesDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge ein Rechteck shape mit korrekten Parametern hinzu
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 0);

            // Setze den Soft-Edges-Effekt mit einem Radius von 5 Punkten (0,5d = 5 Punkte)
            shape.SoftEdges = 0.5d;

            // Speichere die Arbeitsmappe
            workbook.Save("SoftEdgesDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


