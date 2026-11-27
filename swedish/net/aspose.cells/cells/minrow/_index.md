---
title: "Cells.MinRow"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cells-egenskap. Minsta radindex för en cell som innehåller data eller stil"
type: docs
url: /sv/net/aspose.cells/cells/minrow/
---
## Cells.MinRow property

Minsta radindex för cellen som innehåller data eller stil.

```csharp
public int MinRow { get; }
```

### Anmärkningar

Denna egenskap måste iterera och kontrollera celler och rader dynamiskt, så det är en tidskrävande process och bör inte anropas upprepade gånger, till exempel genom att använda den direkt som villkor i en loop.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyMinRowDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Lägg till lite data för att demonstrera MinRow
            cells["A1"].PutValue("Data in first row");
            cells["B5"].PutValue("Data in fifth row");

            // Visa MinRow-information
            Console.WriteLine("Minimum used row: " + cells.MinRow);
            Console.WriteLine("Maximum used row: " + cells.MaxRow);

            // Rensa innehåll med start från MinRow
            cells.ClearContents(cells.MinRow, cells.MinColumn, cells.MaxRow, cells.MaxColumn);

            // Verifiera rensning genom att kontrollera om cellerna är tomma
            Console.WriteLine("A1 after clearing: " + (cells["A1"].Value == null ? "Empty" : "Not empty"));
            Console.WriteLine("B5 after clearing: " + (cells["B5"].Value == null ? "Empty" : "Not empty"));
        }
    }
}
```

### Se även

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


