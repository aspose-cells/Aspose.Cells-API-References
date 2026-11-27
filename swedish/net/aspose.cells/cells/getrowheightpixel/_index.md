---
title: "Cells.GetRowHeightPixel"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cells-metod. Hämtar höjden på en specificerad rad i enheten pixel"
type: docs
url: /sv/net/aspose.cells/cells/getrowheightpixel/
---
## Cells.GetRowHeightPixel method

Hämtar höjden på en specificerad rad i enhet pixel.

```csharp
public int GetRowHeightPixel(int row)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| row | Int32 | Radindex |

### Returvärde

Radhöjd

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGetRowHeightPixelWithInt32Demo
    {
        public static void Run()
        {
            // Instansiera en ny arbetsbok
            Workbook wb = new Workbook();

            // Hämta det första kalkylbladet
            Worksheet worksheet = wb.Worksheets[0];

            // Ange radhöjd för rad 5 (i pixlar)
            worksheet.Cells.SetRowHeightPixel(5, 30);

            // Hämta radhöjd för rad 5 (i pixlar)
            int rowHeight = worksheet.Cells.GetRowHeightPixel(5);

            Console.WriteLine("Row height of row 5 in pixels: " + rowHeight);
        }
    }
}
```

### Se även

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


