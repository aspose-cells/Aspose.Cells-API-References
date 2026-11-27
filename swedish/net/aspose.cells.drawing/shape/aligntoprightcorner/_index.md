---
title: "Shape.AlignTopRightCorner"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Shape metod. Flyttar bilden till det övre högra hörnet"
type: docs
url: /sv/net/aspose.cells.drawing/shape/aligntoprightcorner/
---
## Shape.AlignTopRightCorner method

Flyttar bilden till det övre högra hörnet.

```csharp
public void AlignTopRightCorner(int topRow, int rightColumn)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| topRow | Int32 | radindexet. |
| rightColumn | Int32 | kolumnindexet. |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodAlignTopRightCornerWithInt32Int32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en exempelform för att justera
            Shape shape = worksheet.Shapes.AddRectangle(10, 10, 100, 100, 0, 0);

            // Justera formens övre högra hörn till rad 2, kolumn 5
            shape.AlignTopRightCorner(2, 5);

            // Spara arbetsboken
            workbook.Save("AlignTopRightCornerDemo.xlsx");
        }
    }
}
```

### Se även

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


