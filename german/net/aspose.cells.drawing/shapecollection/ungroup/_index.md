---
title: "ShapeCollection.Ungroup"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ShapeCollection-Methode. Entgruppiert die Formelemente."
type: docs
url: /de/net/aspose.cells.drawing/shapecollection/ungroup/
---
## ShapeCollection.Ungroup method

Löst die Gruppierung der Shape-Elemente auf.

```csharp
public void Ungroup(GroupShape group)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Gruppe | GroupShape | Die Gruppenform. |

### Hinweise

Wenn die Gruppenform von einer anderen Gruppenform gruppiert ist,nichts wird getan.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodUngroupWithGroupShapeDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Rufe die Formensammlung ab
            ShapeCollection shapes = worksheet.Shapes;

            // Erste Rechteckform hinzufügen
            shapes.AddRectangle(2, 0, 2, 0, 50, 50);
            
            // Zweite Rechteckform hinzufügen
            shapes.AddRectangle(6, 0, 2, 0, 30, 30);

            // Array von Formen zum Gruppieren erstellen
            Shape[] shapesArr = new Shape[] { shapes[0], shapes[1] };

            // Gruppiere die Formen
            GroupShape groupShape = shapes.Group(shapesArr);

            // Entgruppiere die Gruppenform
            shapes.Ungroup(groupShape);
        }
    }
}
```

### Siehe auch

* class [GroupShape](../../groupshape/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


