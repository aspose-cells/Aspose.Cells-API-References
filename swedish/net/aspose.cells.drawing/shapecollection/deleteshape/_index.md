---
title: "ShapeCollection.DeleteShape"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ShapeCollection metod. Ta bort en form. Om formen är i gruppen eller är en kommentarsform tas den inte bort."
type: docs
url: /sv/net/aspose.cells.drawing/shapecollection/deleteshape/
---
## ShapeCollection.DeleteShape method

Ta bort en form. Om formen är i en grupp eller är en kommentarsform, kommer den inte att tas bort.

```csharp
public void DeleteShape(Shape shape)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| form | Form |  |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodDeleteShapeWithShapeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Hämta samlingen av former
            ShapeCollection shapes = worksheet.Shapes;

            // Lägg till den första rektangelformen
            Shape firstShape = shapes.AddRectangle(2, 0, 2, 0, 50, 50);
            
            // Lägg till den andra rektangelformen
            Shape secondShape = shapes.AddRectangle(6, 0, 2, 0, 30, 30);

            // Ta bort den första formen
            shapes.DeleteShape(firstShape);

            // Spara arbetsboken
            workbook.Save("DeleteShapeDemo.xlsx");
        }
    }
}
```

### Se även

* class [Shape](../../shape/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


