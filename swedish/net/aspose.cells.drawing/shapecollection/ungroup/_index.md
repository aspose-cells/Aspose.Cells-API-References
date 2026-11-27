---
title: "ShapeCollection.Ungroup"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ShapeCollection-metod. Avgrupperar formobjekten"
type: docs
url: /sv/net/aspose.cells.drawing/shapecollection/ungroup/
---
## ShapeCollection.Ungroup method

Avgrupperar formobjekten.

```csharp
public void Ungroup(GroupShape group)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| grupp | GroupShape | Gruppformen. |

### Anmärkningar

Om gruppformen är grupperad av en annan gruppform, görs inget.

### Exempel

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
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Hämta samlingen av former
            ShapeCollection shapes = worksheet.Shapes;

            // Lägg till den första rektangelformen
            shapes.AddRectangle(2, 0, 2, 0, 50, 50);
            
            // Lägg till den andra rektangelformen
            shapes.AddRectangle(6, 0, 2, 0, 30, 30);

            // Skapa en array av former att gruppera
            Shape[] shapesArr = new Shape[] { shapes[0], shapes[1] };

            // Gruppera formerna
            GroupShape groupShape = shapes.Group(shapesArr);

            // Avgruppera gruppformen
            shapes.Ungroup(groupShape);
        }
    }
}
```

### Se även

* class [GroupShape](../../groupshape/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


