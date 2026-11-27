---
title: "Cells.GetMaxGroupedColumnOutlineLevel"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cells-metoden. Hämtar den maximala grupperade kolumnens konturnivå, nollbaserad"
type: docs
url: /sv/net/aspose.cells/cells/getmaxgroupedcolumnoutlinelevel/
---
## Cells.GetMaxGroupedColumnOutlineLevel method

Hämtar den maximala grupperade kolumnens konturnivå (nollbaserad).

```csharp
public int GetMaxGroupedColumnOutlineLevel()
```

### Returvärde

Den maximala grupperade kolumnens konturnivå (nollbaserad)

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGetMaxGroupedColumnOutlineLevelDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Gruppera några kolumner för att demonstrera konturnivåer
            cells.GroupColumns(0, 2, false);
            cells.GroupColumns(3, 5, false);
            
            // Hämta den maximala grupperade kolumnens konturnivå
            int maxOutlineLevel = cells.GetMaxGroupedColumnOutlineLevel();
            
            Console.WriteLine("Maximum grouped column outline level: " + maxOutlineLevel);
            
            // Visa konturnivå för varje kolumn
            for (int col = 0; col < 6; col++)
            {
                int outlineLevel = cells.GetGroupedColumnOutlineLevel(col);
                Console.WriteLine($"Column {col} outline level: {outlineLevel}");
            }
            
            // Spara arbetsboken
            workbook.Save("GroupedColumnsOutlineLevel.xlsx");
        }
    }
}
```

### Se även

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


