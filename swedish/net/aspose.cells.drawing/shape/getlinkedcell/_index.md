---
title: "Shape.GetLinkedCell"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Shape method. Hämtar intervallet som är länkat till kontrollens värde"
type: docs
url: /sv/net/aspose.cells.drawing/shape/getlinkedcell/
---
## Shape.GetLinkedCell method

Hämtar intervallet som är länkat till kontrollens värde.

```csharp
public string GetLinkedCell(bool isR1C1, bool isLocal)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| isR1C1 | Boolean | Om formeln behöver formateras som R1C1. |
| isLocal | Boolean | Om formeln behöver formateras enligt lokala inställningar. |

### Returvärde

Intervallet som är länkat till kontrollens värde.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodGetLinkedCellWithBooleanBooleanDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en shape och ställ in dess länkade cell
            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 0, 0);
            shape.LinkedCell = "A1";

            // Hämta den länkade cellens adress med olika parameterkombinationer
            string link1 = shape.GetLinkedCell(false, false); // Returns absolute reference like "$A$1"
            string link2 = shape.GetLinkedCell(true, false);   // Returns relative reference like "A1"
            string link3 = shape.GetLinkedCell(false, true);   // Returns R1C1 style absolute reference

            Console.WriteLine("Linked cell (absolute A1): " + link1);
            Console.WriteLine("Linked cell (relative A1): " + link2);
            Console.WriteLine("Linked cell (R1C1 style): " + link3);
        }
    }
}
```

### Se även

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


