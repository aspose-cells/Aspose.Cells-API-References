---
title: "Cells.GetGroupedRowOutlineLevel"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cells-metod. Hämtar radens konturnivå nollbaserad."
type: docs
url: /sv/net/aspose.cells/cells/getgroupedrowoutlinelevel/
---
## Cells.GetGroupedRowOutlineLevel method

Hämtar konturnivån (nollbaserad) för raden.

```csharp
public int GetGroupedRowOutlineLevel(int rowIndex)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rowIndex | Int32 | Radindexet. |

### Returvärde

Radens konturnivå (nollbaserad).

### Anmärkningar

Om raden inte är grupperad returneras noll.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGetGroupedRowOutlineLevelWithInt32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Gruppera rader 0-3 (nivå 1)
            cells.GroupRows(0, 3, false);
            
            // Gruppera rader 0-1 (nivå 2)
            cells.GroupRows(0, 1, false);

            // Hämta konturnivå för varje rad
            for (int row = 0; row <= 4; row++)
            {
                int outlineLevel = cells.GetGroupedRowOutlineLevel(row);
                Console.WriteLine($"Row {row} outline level: {outlineLevel}");
            }

            // Avgruppera alla rader
            cells.UngroupRows(0, 3);
        }
    }
}
```

### Se även

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


