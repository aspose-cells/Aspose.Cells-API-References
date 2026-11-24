---
title: "ShapeCollection.Group"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ShapeCollection-Methode. Gruppiere die Formen"
type: docs
url: /de/net/aspose.cells.drawing/shapecollection/group/
---
## ShapeCollection.Group method

Gruppiere die Shapes.

```csharp
public GroupShape Group(Shape[] groupItems)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| groupItems | Shape[] | die Gruppenelemente. |

### Rückgabewert

Gibt die Gruppenform zurück.

### Hinweise

Die Form in den groupItems sollte nicht gruppiert werden. Die Form muss in dieser Shapes-Sammlung sein.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodGroupWithShapeArrayDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Rufe die Formensammlung ab
            ShapeCollection shapes = worksheet.Shapes;

            // Erste Rechteckform hinzufügen
            shapes.AddRectangle(2, 0, 2, 0, 50, 50);
            
            // Zweite Rechteckform hinzufügen
            shapes.AddRectangle(6, 0, 2, 0, 30, 30);

            // Array mit den zu gruppierenden Formen erstellen
            Shape[] shapesArr = new Shape[] { shapes[0], shapes[1] };

            // Gruppiere die Formen
            GroupShape groupShape = shapes.Group(shapesArr);

            // Speichere die Arbeitsmappe
            workbook.Save("GroupShapesDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [GroupShape](../../groupshape/)
* class [Shape](../../shape/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


