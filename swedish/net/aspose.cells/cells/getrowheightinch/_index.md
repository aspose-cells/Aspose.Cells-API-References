---
title: "Cells.GetRowHeightInch"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cells-metod. Hämtar höjden på en specificerad rad i tum."
type: docs
url: /sv/net/aspose.cells/cells/getrowheightinch/
---
## Cells.GetRowHeightInch method

Hämtar höjden på en specificerad rad i enhet tum.

```csharp
public double GetRowHeightInch(int row)
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
    public class CellsMethodGetRowHeightInchWithInt32Demo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Ställ in radhöjd i tum för rad 5
            cells.SetRowHeightInch(5, 1.5);

            // Hämta radhöjd i tum för rad 5
            double rowHeight = cells.GetRowHeightInch(5);

            // Skriv ut resultatet
            Console.WriteLine("Row height in inches: " + rowHeight);
        }
    }
}
```

### Se även

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


