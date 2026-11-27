---
title: "Cells.GetViewRowHeight"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cells-metod. Hämtar höjden på en angiven rad"
type: docs
url: /sv/net/aspose.cells/cells/getviewrowheight/
---
## Cells.GetViewRowHeight method

Hämtar höjden på en specificerad rad.

```csharp
public double GetViewRowHeight(int row)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| row | Int32 | Radindex. |

### Returvärde

Radens höjd.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGetViewRowHeightWithInt32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ställ in radens höjd för rad 3 (i punkter)
            worksheet.Cells.SetRowHeight(3, 15);
            
            // Hämta visningsradens höjd för rad 3
            double viewRowHeight = worksheet.Cells.GetViewRowHeight(3);
            
            // Skriv ut resultatet
            Console.WriteLine("View Row Height for row 3: " + viewRowHeight);
        }
    }
}
```

### Se även

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


