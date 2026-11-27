---
title: "ShapeCollection.Group"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ShapeCollection-metod. Gruppera formerna"
type: docs
url: /sv/net/aspose.cells.drawing/shapecollection/group/
---
## ShapeCollection.Group method

Gruppera formerna.

```csharp
public GroupShape Group(Shape[] groupItems)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| groupItems | Shape[] | gruppobjekten. |

### Returvärde

Returnerar gruppformen.

### Anmärkningar

Formen i groupItems bör inte grupperas. Formen måste finnas i den här Shapes-samlingen.

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Hämta samlingen av former
            ShapeCollection shapes = worksheet.Shapes;

            // Lägg till den första rektangelformen
            shapes.AddRectangle(2, 0, 2, 0, 50, 50);
            
            // Lägg till den andra rektangelformen
            shapes.AddRectangle(6, 0, 2, 0, 30, 30);

            // Skapa en array med formerna att gruppera
            Shape[] shapesArr = new Shape[] { shapes[0], shapes[1] };

            // Gruppera formerna
            GroupShape groupShape = shapes.Group(shapesArr);

            // Spara arbetsboken
            workbook.Save("GroupShapesDemo.xlsx");
        }
    }
}
```

### Se även

* class [GroupShape](../../groupshape/)
* class [Shape](../../shape/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


