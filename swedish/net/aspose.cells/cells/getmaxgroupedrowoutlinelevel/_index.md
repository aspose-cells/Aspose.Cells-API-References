---
title: "Cells.GetMaxGroupedRowOutlineLevel"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cells-metod. Hämtar den maximala grupperade radens konturnivå nollbaserad"
type: docs
url: /sv/net/aspose.cells/cells/getmaxgroupedrowoutlinelevel/
---
## Cells.GetMaxGroupedRowOutlineLevel method

Hämtar den maximala grupperade radens konturnivå (nollbaserad).

```csharp
public int GetMaxGroupedRowOutlineLevel()
```

### Returvärde

Den maximala grupperade radens konturnivå (nollbaserad)

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGetMaxGroupedRowOutlineLevelDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Gruppera några rader för att demonstrera konturnivåer
            cells.GroupRows(0, 2, false);
            cells.GroupRows(4, 6, false);
            
            // Lägg till nästlad gruppering
            cells.GroupRows(4, 5, true);

            // Hämta den maximala grupperade radens konturnivå
            int maxOutlineLevel = cells.GetMaxGroupedRowOutlineLevel();

            // Visa resultatet
            Console.WriteLine("Maximum grouped row outline level: " + maxOutlineLevel);

            // Visa konturnivå för varje rad
            for (int row = 0; row <= 6; row++)
            {
                Console.WriteLine($"Row {row} outline level: {cells.GetGroupedRowOutlineLevel(row)}");
            }
        }
    }
}
```

### Se även

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


