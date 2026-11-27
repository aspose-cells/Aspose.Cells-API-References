---
title: "ShapeCollection.DeleteInRange"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ShapeCollection-metod. Ta bort former i intervallet. Kommentarformer kommer inte att tas bort"
type: docs
url: /sv/net/aspose.cells.drawing/shapecollection/deleteinrange/
---
## ShapeCollection.DeleteInRange method

Ta bort former i området. Kommentarsformer kommer inte att tas bort.

```csharp
public void DeleteInRange(CellArea ca)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| ca | CellArea | Intervallet. Om formerna finns i intervallet, tas de bort. |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodDeleteInRangeWithCellAreaDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            ShapeCollection shapes = worksheet.Shapes;

            // Lägg till den första rektangelformen
            shapes.AddRectangle(2, 0, 2, 0, 50, 50);
            // Lägg till den andra rektangelformen
            shapes.AddRectangle(6, 0, 2, 0, 30, 30);

            // Definiera intervallet där former ska tas bort
            CellArea area = new CellArea();
            area.StartColumn = 0;
            area.StartRow = 5;
            area.EndColumn = 5;
            area.EndRow = 8;

            // Ta bort former inom det angivna intervallet
            shapes.DeleteInRange(area);

            // Spara arbetsboken (valfritt)
            workbook.Save("ShapeDeleteInRangeDemo.xlsx");
        }
    }
}
```

### Se även

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


