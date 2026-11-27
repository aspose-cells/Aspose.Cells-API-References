---
title: "CellWatch.Row"
second_title: "Aspose.Cells för .NET API‑referens"
description: "CellWatch-egenskap. Hämtar och anger raden för cellen"
type: docs
url: /sv/net/aspose.cells/cellwatch/row/
---
## CellWatch.Row property

Hämtar och anger raden för cellen.

```csharp
public int Row { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellWatchPropertyRowDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till exempeldata i cell B2
            sheet.Cells["B2"].PutValue("Sample Data");

            // Lägg till CellWatch för B2
            int watchIndex = sheet.CellWatches.Add("B2");
            CellWatch cellWatch = sheet.CellWatches[watchIndex];

            // Demonstrera Row-egenskapen
            Console.WriteLine($"Original Row: {cellWatch.Row}");
            cellWatch.Row = 1; // Set row to 1 (0-based) for B2
            Console.WriteLine($"Updated Row: {cellWatch.Row}");

            // Verifiera cellreferensen
            Console.WriteLine($"Cell Reference: {sheet.Cells[cellWatch.Row, cellWatch.Column].Name}");

            workbook.Save("CellWatchRowDemo.xlsx");
        }
    }
}
```

### Se även

* class [CellWatch](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


