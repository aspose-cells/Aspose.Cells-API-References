---
title: "Klass CellWatch"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.CellWatch-klass. Representerar Cell Watch‑objekt i övervakningsfönstret"
type: docs
url: /sv/net/aspose.cells/cellwatch/
---
## CellWatch class

Representerar Cell Watch Item i 'watch window'.

```csharp
public class CellWatch
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [CellWatch](cellwatch/)() | Standardkonstruktorn. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [CellName](../../aspose.cells/cellwatch/cellname/) { get; set; } | Hämtar och anger namnet på cellen. |
| [Column](../../aspose.cells/cellwatch/column/) { get; set; } | Hämtar och anger kolumnen för cellen. |
| [Row](../../aspose.cells/cellwatch/row/) { get; set; } | Hämtar och anger raden för cellen. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellWatchDemo
    {
        public static void CellWatchExample()
        {
            // Instansiering av ett Workbook-objekt
            Workbook workbook = new Workbook();
            // Hämta det första kalkylbladet.
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till Cell Watch‑objekt i övervakningsfönstret
            int watchIndex = sheet.CellWatches.Add("B2");

            // Hämta CellWatch‑objektet
            CellWatch cellWatch = sheet.CellWatches[watchIndex];

            // Ställa in egenskaper
            cellWatch.Row = 1; // B2 corresponds to row 1 (0-based index)
            cellWatch.Column = 1; // B2 corresponds to column 1 (0-based index)
            cellWatch.CellName = "B2";

            // Spara arbetsboken
            workbook.Save("CellWatchExample.xlsx");
            workbook.Save("CellWatchExample.pdf");
            return;
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


