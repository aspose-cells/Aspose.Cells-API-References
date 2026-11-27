---
title: "Cells.MinDataRow"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cells-egenskap. Minsta radindex för cell som innehåller data"
type: docs
url: /sv/net/aspose.cells/cells/mindatarow/
---
## Cells.MinDataRow property

Minsta radindex för cellen som innehåller data.

```csharp
public int MinDataRow { get; }
```

### Anmärkningar

Returnera -1 om det inte finns någon cell som innehåller data. Denna egenskap måste iterera och kontrollera celler och rader dynamiskt, så det är en tidskrävande process och bör inte anropas upprepade gånger, till exempel genom att använda den direkt som villkor i en loop.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyMinDataRowDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Fyll i lite data
            sheet.Cells[0, 0].Value = "Header1";
            sheet.Cells[0, 1].Value = "Header2";
            sheet.Cells[1, 0].Value = "Data1";
            sheet.Cells[1, 1].Value = "Data2";
            sheet.Cells[2, 0].Value = "Data3";
            sheet.Cells[2, 1].Value = "Data4";

            // Demonstrera användning av MinDataRow
            Console.WriteLine("Minimum data row index: " + sheet.Cells.MinDataRow);
            Console.WriteLine("Maximum data row index: " + sheet.Cells.MaxDataRow);

            // Spara arbetsboken
            workbook.Save("MinDataRowExample.xlsx");
        }
    }
}
```

### Se även

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


