---
title: "Shape.HeightInShape"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Shape-Eigenschaft. Gibt den vertikalen Abstand der Form vom oberen Rand der übergeordneten Form in Einheiten von 1/4000 der Höhe der übergeordneten Form an."
type: docs
url: /de/net/aspose.cells.drawing/shape/heightinshape/
---
## Shape.HeightInShape property

Stellt den vertikalen Versatz des Shapes von der oberen Kante des übergeordneten Shapes dar, in Einheiten von 1/4000 der Höhe des übergeordneten Shapes

```csharp
public int HeightInShape { get; set; }
```

### Hinweise

Gilt nur, wenn diese Form in einer Gruppe oder einem Diagramm ist.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyHeightInShapeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge zuerst Formen mit allen erforderlichen Parametern hinzu
            Shape rectangle = worksheet.Shapes.AddRectangle(0, 0, 100, 100, 10, 10);
            Shape oval = worksheet.Shapes.AddOval(0, 0, 100, 100, 10, 120);

            // Gruppiere die Formen
            Shape[] shapes = { rectangle, oval };
            GroupShape groupShape = worksheet.Shapes.Group(shapes);

            // Setze die Höhe des Rechtecks relativ zur übergeordneten Gruppierungsform (1/4000 der übergeordneten Höhe)
            rectangle.HeightInShape = 2000; // Half the height of the parent
            oval.HeightInShape = 4000; // Full height of the parent

            // Speichere die Arbeitsmappe
            workbook.Save("ShapeHeightInShapeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


