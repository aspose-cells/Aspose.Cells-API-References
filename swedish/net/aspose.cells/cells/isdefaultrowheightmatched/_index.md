---
title: "Cells.IsDefaultRowHeightMatched"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cells-egenskap. Indikerar att radhöjden och standardteckensnittshöjden matchar"
type: docs
url: /sv/net/aspose.cells/cells/isdefaultrowheightmatched/
---
## Cells.IsDefaultRowHeightMatched property

Indikerar att radhöjd och standardteckensnittshöjd matchar

```csharp
public bool IsDefaultRowHeightMatched { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyIsDefaultRowHeightMatchedDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;

            // Ställ in och demonstrera IsDefaultRowHeightMatched-egenskapen
            cells.IsDefaultRowHeightMatched = true;
            Console.WriteLine("IsDefaultRowHeightMatched: " + cells.IsDefaultRowHeightMatched);

            // Spara arbetsboken
            workbook.Save("output.xlsx");

            // Läs in den sparade arbetsboken för att verifiera egenskapen
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            Cells loadedCells = loadedWorkbook.Worksheets[0].Cells;
            Console.WriteLine("Loaded IsDefaultRowHeightMatched: " + loadedCells.IsDefaultRowHeightMatched);
        }
    }
}
```

### Se även

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


