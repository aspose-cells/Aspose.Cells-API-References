---
title: "Cells.MaxColumn"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cells-egenskap. Största kolumnindex för de celler som har instansierats i samlingen, inkluderar inte den kolumn där stil är definierad för hela kolumnen men ingen cell har instansierats i den."
type: docs
url: /sv/net/aspose.cells/cells/maxcolumn/
---
## Cells.MaxColumn property

Maximalt kolumnindex för de celler som har instansierats i samlingen (inkluderar inte kolumnen där stil är definierad för hela kolumnen men ingen cell har instansierats i den).

```csharp
public int MaxColumn { get; }
```

### Anmärkningar

Returnera -1 om ingen cell har instansierats.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyMaxColumnDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till lite data i cellerna
            worksheet.Cells["A1"].PutValue("Column A");
            worksheet.Cells["B1"].PutValue("Column B");
            worksheet.Cells["C1"].PutValue("Column C");
            
            // Hämta det största kolumnindexet med data
            int maxColumn = worksheet.Cells.MaxColumn;
            Console.WriteLine("Max column with data: " + maxColumn);

            // Lägg till data i nästa kolumn efter maxkolumnen
            worksheet.Cells[0, maxColumn + 1].PutValue("Next Column");

            // Verifiera den nya maxkolumnen
            Console.WriteLine("New max column: " + worksheet.Cells.MaxColumn);

            // Skapa ett annat kalkylblad för att demonstrera kopiering
            Worksheet destSheet = workbook.Worksheets.Add("Destination");

            // Kopiera alla kolumner från källan till destinationen
            destSheet.Cells.CopyColumns(worksheet.Cells, 0, 0, worksheet.Cells.MaxColumn + 1);

            Console.WriteLine("Columns copied successfully");
        }
    }
}
```

### Se även

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


