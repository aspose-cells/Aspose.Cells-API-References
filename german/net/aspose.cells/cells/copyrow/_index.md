---
title: "Cells.CopyRow"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cells‑Methode. Kopiert Daten und Formate einer gesamten Zeile."
type: docs
url: /de/net/aspose.cells/cells/copyrow/
---
## Cells.CopyRow method

Kopiert Daten und Formate einer ganzen Zeile.

```csharp
public void CopyRow(Cells sourceCells, int sourceRowIndex, int destinationRowIndex)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sourceCells | Zellen | Quell‑Cells‑Objekt enthält zu kopierende Daten und Formate. |
| sourceRowIndex | Int32 | Quell‑Zeilenindex. |
| destinationRowIndex | Int32 | Zielzeilenindex. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodCopyRowWithCellsInt32Int32Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet1 = workbook.Worksheets[0];
            Cells cells1 = worksheet1.Cells;
            
            // Fügen Sie einige Daten zur ersten Zeile hinzu
            cells1["A1"].PutValue("Source Data");
            cells1["B1"].PutValue(100);
            cells1["C1"].PutValue(DateTime.Now);
            
            // Zweites Arbeitsblatt erstellen
            Worksheet worksheet2 = workbook.Worksheets.Add("Sheet2");
            Cells cells2 = worksheet2.Cells;
            
            // Zeile von Sheet1 nach Sheet2 kopieren
            cells2.CopyRow(cells1, 0, 0);
            
            // Zeile innerhalb von Sheet1 an neue Positionen kopieren
            cells1.CopyRow(cells1, 0, 1);
            cells1.CopyRow(cells1, 0, 2);
            
            // Speichere die Arbeitsmappe
            workbook.Save("CopyRowExample.xlsx");
        }
    }
}
```

### Siehe auch

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


