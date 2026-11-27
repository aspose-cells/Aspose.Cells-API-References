---
title: "Cells.CopyRow"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cells-metod. Kopierar data och format för en hel rad"
type: docs
url: /sv/net/aspose.cells/cells/copyrow/
---
## Cells.CopyRow method

Kopierar data och format för en hel rad.

```csharp
public void CopyRow(Cells sourceCells, int sourceRowIndex, int destinationRowIndex)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sourceCells | Celler | Source Cells-objektet innehåller data och format att kopiera. |
| sourceRowIndex | Int32 | Källradens index. |
| destinationRowIndex | Int32 | Målradsindex. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodCopyRowWithCellsInt32Int32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet1 = workbook.Worksheets[0];
            Cells cells1 = worksheet1.Cells;
            
            // Lägg till lite data i den första raden
            cells1["A1"].PutValue("Source Data");
            cells1["B1"].PutValue(100);
            cells1["C1"].PutValue(DateTime.Now);
            
            // Skapa ett andra arbetsblad
            Worksheet worksheet2 = workbook.Worksheets.Add("Sheet2");
            Cells cells2 = worksheet2.Cells;
            
            // Kopiera rad från Sheet1 till Sheet2
            cells2.CopyRow(cells1, 0, 0);
            
            // Kopiera rad inom Sheet1 till nya positioner
            cells1.CopyRow(cells1, 0, 1);
            cells1.CopyRow(cells1, 0, 2);
            
            // Spara arbetsboken
            workbook.Save("CopyRowExample.xlsx");
        }
    }
}
```

### Se även

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


