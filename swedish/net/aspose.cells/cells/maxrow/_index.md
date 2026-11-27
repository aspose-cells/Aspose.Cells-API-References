---
title: "Cells.MaxRow"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cells-egenskap. Maximalt radindex för cell som innehåller data eller stil"
type: docs
url: /sv/net/aspose.cells/cells/maxrow/
---
## Cells.MaxRow property

Maximalt radindex för celler som innehåller data eller stil.

```csharp
public int MaxRow { get; }
```

### Anmärkningar

Returnera -1 om det inte finns någon cell som innehåller data eller stil i kalkylbladet. Denna egenskap måste iterera och kontrollera celler och rader dynamiskt, så det är en tidskrävande process och bör inte anropas upprepade gånger, till exempel genom att använda den direkt som villkor i en loop.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyMaxRowDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Lägg till lite exempeldata
            cells[0, 0].PutValue("Name");
            cells[0, 1].PutValue("Age");
            cells[1, 0].PutValue("John");
            cells[1, 1].PutValue(30);
            cells[2, 0].PutValue("Alice");
            cells[2, 1].PutValue(25);

            // Hämta det maximala radindexet (nollbaserat)
            int maxRow = cells.MaxRow;
            Console.WriteLine("MaxRow before adding new data: " + maxRow);

            // Lägg till ny data i nästa rad efter den maximala raden
            int newRow = maxRow + 1;
            cells[newRow, 0].PutValue("Bob");
            cells[newRow, 1].PutValue(28);

            // Verifiera den nya maximala raden
            Console.WriteLine("MaxRow after adding new data: " + cells.MaxRow);

            // Spara arbetsboken
            workbook.Save("MaxRowDemo.xlsx");
        }
    }
}
```

### Se även

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


