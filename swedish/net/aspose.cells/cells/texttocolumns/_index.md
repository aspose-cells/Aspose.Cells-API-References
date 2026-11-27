---
title: "Cells.TextToColumns"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cells method. Delar upp innehåll i angiven kolumn i flera kolumner"
type: docs
url: /sv/net/aspose.cells/cells/texttocolumns/
---
## Cells.TextToColumns method

Delar upp innehållet i angiven kolumn i flera kolumner..

```csharp
public int TextToColumns(int row, int column, int totalRows, TxtLoadOptions options)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| row | Int32 | Radindexet. |
| column | Int32 | Kolumnindexet. |
| totalRows | Int32 | Antalet rader. |
| alternativ | TxtLoadOptions | Delningsalternativen. |

### Returvärde

Totalt antal kolumner för de delade värdena.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodTextToColumnsWithInt32Int32Int32TxtLoadOptionsDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Ange exempeldata med kommaseparerade värden
            sheet.Cells["A1"].PutValue("John,Doe,30");
            sheet.Cells["A2"].PutValue("Jane,Smith,28");

            // Skapa textinläsningsalternativ med komma som avgränsare
            TxtLoadOptions options = new TxtLoadOptions();
            options.Separator = ',';

            // Dela upp text till kolumner med start från cell A1, 3 kolumner bred
            sheet.Cells.TextToColumns(0, 0, 3, options);

            // Verifiera resultaten
            Console.WriteLine("B1: " + sheet.Cells["B1"].StringValue); // Should output "Doe"
            Console.WriteLine("C2: " + sheet.Cells["C2"].StringValue); // Should output "28"

            // Spara arbetsboken
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [TxtLoadOptions](../../txtloadoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


