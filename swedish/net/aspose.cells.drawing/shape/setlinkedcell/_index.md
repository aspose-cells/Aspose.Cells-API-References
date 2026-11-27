---
title: "Shape.SetLinkedCell"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Shape-metod. Ställer in intervallet som är länkat till kontrollens värde"
type: docs
url: /sv/net/aspose.cells.drawing/shape/setlinkedcell/
---
## Shape.SetLinkedCell method

Ställer in intervallet som är länkat till kontrollens värde.

```csharp
public void SetLinkedCell(string formula, bool isR1C1, bool isLocal)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| formel | String | Intervallet som är länkat till kontrollens värde. |
| isR1C1 | Boolean | Om formeln behöver formateras som R1C1. |
| isLocal | Boolean | Om formeln behöver formateras enligt lokala inställningar. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ShapeMethodSetLinkedCellWithStringBooleanBooleanDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en rullningslistform
            Aspose.Cells.Drawing.Shape scrollBar = worksheet.Shapes.AddScrollBar(2, 0, 2, 0, 130, 30);

            // Länka rullningslistens värde till cell A12
            scrollBar.SetLinkedCell("$A$12", false, true);

            // Spara arbetsboken
            workbook.Save("SetLinkedCellDemo.xlsx");
        }
    }
}
```

### Se även

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


