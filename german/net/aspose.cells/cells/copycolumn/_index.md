---
title: "Cells.CopyColumn"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cells-Methode. Kopiert Daten und Formate einer gesamten Spalte"
type: docs
url: /de/net/aspose.cells/cells/copycolumn/
---
## Cells.CopyColumn method

Kopiert Daten und Formate einer ganzen Spalte.

```csharp
public void CopyColumn(Cells sourceCells, int sourceColumnIndex, int destinationColumnIndex)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sourceCells | Zellen | Quell‑Cells‑Objekt enthält zu kopierende Daten und Formate. |
| sourceColumnIndex | Int32 | Index der Quellspalte. |
| destinationColumnIndex | Int32 | Zielspaltenindex. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodCopyColumnWithCellsInt32Int32Demo
    {
        public static void Run()
        {
            // Erstelle die Quellarbeitsmappe und fülle Daten.
            Workbook wbSrc = new Workbook();
            Cells cellsSrc = wbSrc.Worksheets[0].Cells;
            cellsSrc[0, 255].PutValue(1);
            cellsSrc[1, 255].PutValue(true);
            cellsSrc[2, 255].PutValue("abc");
            cellsSrc[3, 255].PutValue(false);
            cellsSrc[65535, 255].PutValue(2.56);

            // Erstelle Ziel‑Arbeitsbuch
            Workbook wbDest = new Workbook();
            Cells cellsDest = wbDest.Worksheets[0].Cells;

            // Kopiere die Spalte von der Quelle zum Ziel.
            cellsDest.CopyColumn(cellsSrc, 255, 0);

            // Ergebnis speichern
            wbDest.Save("outputCopyColumn.xlsx");
            
            Console.WriteLine("Column copied successfully.");
        }
    }
}
```

### Siehe auch

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


