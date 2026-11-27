---
title: "Cells.SetRowHeightPixel"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cells-metod. Anger radhöjden i pixelenheter"
type: docs
url: /sv/net/aspose.cells/cells/setrowheightpixel/
---
## Cells.SetRowHeightPixel method

Ställer in radens höjd i enhet pixlar.

```csharp
public void SetRowHeightPixel(int row, int pixels)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| row | Int32 | Radindex. |
| pixlar | Int32 | Antal pixlar. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodSetRowHeightPixelWithInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ställ in höjden för första raden till 50 pixlar
            worksheet.Cells.SetRowHeightPixel(0, 50);

            // Ställ in höjden för andra raden till 100 pixlar
            worksheet.Cells.SetRowHeightPixel(1, 100);

            // Spara arbetsboken
            workbook.Save("RowHeightPixelDemo.xlsx");
        }
    }
}
```

### Se även

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


