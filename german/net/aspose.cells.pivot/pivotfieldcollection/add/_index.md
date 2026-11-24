---
title: "PivotFieldCollection.Add"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotFieldCollection‑Methode. Fügt ein PivotField‑Objekt zum spezifischen Typ PivotFields hinzu"
type: docs
url: /de/net/aspose.cells.pivot/pivotfieldcollection/add/
---
## PivotFieldCollection.Add method

Fügt ein PivotField‑Objekt zum spezifischen Typ PivotFields hinzu.

```csharp
public int Add(PivotField pivotField)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| pivotField | PivotField | ein PivotField-Objekt. |

### Rückgabewert

der Index des PivotField-Objekts in diesen PivotFields.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldCollectionMethodAddWithPivotFieldDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe aus einer Quell‑Excel‑Datei
            Workbook workbook = new Workbook("sample_pivot_table.xlsx");
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Greifen Sie auf die erste Pivot-Tabelle zu.
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // Pivot-Tabellendaten aktualisieren
            pivotTable.RefreshData();
            
            // Datenfeld zum Spaltenfeldbereich mit der Add‑Methode hinzufügen
            pivotTable.ColumnFields.Add(pivotTable.DataField);
            
            // PivotTable-Daten berechnen
            pivotTable.CalculateData();
            
            // Speichere die Arbeitsmappe
            workbook.Save("output_pivot_table.xlsx");
        }
    }
}
```

### Siehe auch

* class [PivotField](../../pivotfield/)
* class [PivotFieldCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


