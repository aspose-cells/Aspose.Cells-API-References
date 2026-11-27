---
title: "ShapeCollection.Remove"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ShapeCollection-metod. Ta bort formen"
type: docs
url: /sv/net/aspose.cells.drawing/shapecollection/remove/
---
## ShapeCollection.Remove method

Ta bort formen.

```csharp
public void Remove(Shape shape)
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
    public class ShapeCollectionMethodRemoveWithShapeDemo
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

            // Hämta den första formen efter namn eller index
            Shape shapeToRemove = shapes["Rectangle 1"]; // or shapes[0];
            
            if (shapeToRemove != null)
            {
                // Ta bort formen från samlingen
                shapes.Remove(shapeToRemove);
            }

            // Spara arbetsboken
            workbook.Save("ShapeRemoveDemo.xlsx");
        }
    }
}
```

### Se även

* class [Shape](../../shape/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


