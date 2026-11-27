---
title: "Cells.MinDataColumn"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cells-egenskap. Minsta kolumnindex för en cell som innehåller data"
type: docs
url: /sv/net/aspose.cells/cells/mindatacolumn/
---
## Cells.MinDataColumn property

Minsta kolumnindex för cellen som innehåller data.

```csharp
public int MinDataColumn { get; }
```

### Anmärkningar

-1 will be returned if there is no cell which contains data. This property needs to iterate and check all cells in a worksheet dynamically, so it is a time-consumed progress and should not be invoked repeatedly, such as using it directly as condition in a loop.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyMinDataColumnDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            
            // Lägg till data i celler (börjar från kolumn 2)
            cells["B1"].PutValue("Header1");
            cells["C2"].PutValue("Data1");
            cells["D3"].PutValue("Data2");
            cells["E4"].PutValue("Data3");
            
            // Hämta det minsta kolumnindexet som innehåller data
            int minDataColumn = cells.MinDataColumn;
            
            // Skriv ut resultatet
            Console.WriteLine("Minimum data column index: " + minDataColumn);
        }
    }
}
```

### Se även

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


