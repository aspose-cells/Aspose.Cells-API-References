---
title: "PivotTableFormatCollection.Item"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotTableFormatCollection-Eigenschaft. Gibt das Format anhand des Index zurück"
type: docs
url: /de/net/aspose.cells.pivot/pivottableformatcollection/item/
---
## PivotTableFormatCollection indexer

Ruft das Format über den Index ab.

```csharp
public PivotTableFormat this[int index] { get; }
```

| Parameter | Beschreibung |
| --- | --- |
| Index | Der Index. |

### Beispiele

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableFormatCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe aus einer Quell‑Excel‑Datei
            Workbook workbook = new Workbook("example.xlsx");

            // Alle Pivot-Tabellen aktualisieren
            workbook.Worksheets.RefreshAll();
            Cells cells = workbook.Worksheets[0].Cells;

            // Greifen Sie auf die erste Pivot-Tabelle zu.
            PivotTable pt = workbook.Worksheets[0].PivotTables[0];

            // Demonstrieren Sie die Item-Eigenschaft, indem Sie das erste PivotFormat aufrufen
            pt.PivotFormats[0].PivotArea.OnlyData = false;
            workbook.Worksheets.RefreshAll();

            // Formatierungseinstellungen mit der Item-Eigenschaft ändern
            pt.PivotFormats[0].PivotArea.OnlyLabel = true;
            workbook.Worksheets.RefreshAll();

            // Speichere die geänderte Arbeitsmappe
            workbook.Save("modified_example.xlsx");
        }
    }
}
```

### Siehe auch

* class [PivotTableFormat](../../pivottableformat/)
* class [PivotTableFormatCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


