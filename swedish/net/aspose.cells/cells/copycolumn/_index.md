---
title: "Cells.CopyColumn"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cells-metoden. Kopierar data och format för en hel kolumn"
type: docs
url: /sv/net/aspose.cells/cells/copycolumn/
---
## Cells.CopyColumn method

Kopierar data och format för en hel kolumn.

```csharp
public void CopyColumn(Cells sourceCells, int sourceColumnIndex, int destinationColumnIndex)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sourceCells | Celler | Source Cells-objektet innehåller data och format att kopiera. |
| sourceColumnIndex | Int32 | Källkolumnindex. |
| destinationColumnIndex | Int32 | Destinationskolumnindex. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodCopyColumnWithCellsInt32Int32Demo
    {
        public static void Run()
        {
            // Skapa källarbetsbok och fyll i data
            Workbook wbSrc = new Workbook();
            Cells cellsSrc = wbSrc.Worksheets[0].Cells;
            cellsSrc[0, 255].PutValue(1);
            cellsSrc[1, 255].PutValue(true);
            cellsSrc[2, 255].PutValue("abc");
            cellsSrc[3, 255].PutValue(false);
            cellsSrc[65535, 255].PutValue(2.56);

            // Skapa målarbetsbok
            Workbook wbDest = new Workbook();
            Cells cellsDest = wbDest.Worksheets[0].Cells;

            // Kopiera kolumn från källa till destination
            cellsDest.CopyColumn(cellsSrc, 255, 0);

            // Spara resultatet
            wbDest.Save("outputCopyColumn.xlsx");
            
            Console.WriteLine("Column copied successfully.");
        }
    }
}
```

### Se även

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


