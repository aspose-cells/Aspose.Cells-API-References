---
title: "ShapeCollection.CopyInRange"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ShapeCollection‑metod. Kopierar former i intervallet till destinationsintervallet"
type: docs
url: /sv/net/aspose.cells.drawing/shapecollection/copyinrange/
---
## ShapeCollection.CopyInRange method

Kopiera former i området till målområdet.

```csharp
public void CopyInRange(ShapeCollection sourceShapes, CellArea ca, int destRow, int destColumn, 
    bool isContained)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sourceShapes | ShapeCollection | Källformer. |
| ca | CellArea | Det källintervallet. |
| destRow | Int32 | Destinationsradens index för destinationsintervallet. |
| destColumn | Int32 | Destinationskolumnen för destinationsintervallet. |
| isContained | Boolean | Anger om endast former som finns inom intervallet ska kopieras. Om true kopieras endast formerna i intervallet. Annars fungerar det som i MS Office. |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodCopyInRangeWithShapeCollectionCellAreaInt32InDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Hämta samlingen av former
            ShapeCollection shapes = worksheet.Shapes;

            // Lägg till en rektangelform
            shapes.AddRectangle(2, 0, 2, 0, 130, 130);

            // Definiera cellområdet att kopiera från
            CellArea area2 = new CellArea();
            area2.StartColumn = 1;
            area2.StartRow = 1;
            area2.EndColumn = 5;
            area2.EndRow = 11;

            // Kopiera former inom det angivna intervallet
            shapes.CopyInRange(shapes, area2, 12, 1, false);

            // Spara arbetsboken
            workbook.Save("ShapeCopyDemo.xlsx");
        }
    }
}
```

### Se även

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


