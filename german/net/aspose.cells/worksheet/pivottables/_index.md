---
title: "Worksheet.PivotTables"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Worksheet-Eigenschaft. Gibt alle Pivot-Tabellen in diesem Arbeitsblatt zurück"
type: docs
url: /de/net/aspose.cells/worksheet/pivottables/
---
## Worksheet.PivotTables property

Ruft alle Pivot-Tabellen in diesem Arbeitsblatt ab.

```csharp
public PivotTableCollection PivotTables { get; }
```

### Beispiele

```csharp
using System;
using System.Collections.Generic;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyPivotTablesDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe aus einer Quell‑Excel‑Datei
            Workbook workbook = new Workbook("PivotTableExample.xlsx");
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Zugriff auf die Pivot-Tabellen‑Sammlung aus dem Arbeitsblatt
            PivotTableCollection pivotTables = worksheet.PivotTables;
            
            // Prüfen, ob Pivot-Tabellen vorhanden sind
            if (pivotTables.Count > 0)
            {
                // Erste Pivot-Tabelle abrufen
                PivotTable pivotTable = pivotTables[0];
                
                // Alle vorhandenen Filter löschen
                pivotTable.PivotFilters.Clear();
                
                // Pivot-Tabellendaten aktualisieren
                pivotTable.RefreshData();
                pivotTable.CalculateData();
                
                // Speichere die geänderte Arbeitsmappe
                workbook.Save("PivotTableModified.xlsx");
            }
        }
    }
}
```

### Siehe auch

* class [PivotTableCollection](../../../aspose.cells.pivot/pivottablecollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


