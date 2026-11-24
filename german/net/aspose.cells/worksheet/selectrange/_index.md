---
title: "Worksheet.SelectRange"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Worksheet-Methode. Wählt einen Bereich aus"
type: docs
url: /de/net/aspose.cells/worksheet/selectrange/
---
## Worksheet.SelectRange method

Wählt einen Bereich aus.

```csharp
public void SelectRange(int startRow, int startColumn, int totalRows, int totalColumns, 
    bool removeOthers)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| startRow | Int32 | Die Startzeile. |
| startColumn | Int32 | Die Startspalte |
| totalRows | Int32 | Die Anzahl der Zeilen. |
| totalColumns | Int32 | Die Anzahl der Spalten |
| removeOthers | Boolean | True bedeutet, andere ausgewählte Bereiche zu entfernen und nur diesen Bereich auszuwählen. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodSelectRangeWithInt32Int32Int32Int32BooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Wählen Sie den Bereich von Zeile 1, Spalte 1 bis Zeile 5, Spalte 5 (B2:F6) aus und aktivieren Sie ihn.
            worksheet.SelectRange(1, 1, 5, 5, true);
            
            Console.WriteLine("Active cell: " + worksheet.ActiveCell);
        }
    }
}
```

### Siehe auch

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


