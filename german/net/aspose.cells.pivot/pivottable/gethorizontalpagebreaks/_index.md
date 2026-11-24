---
title: "PivotTable.GetHorizontalPageBreaks"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotTable-Methode. Gibt die horizontalen Seitenumbrüche dieser PivotTable zurück"
type: docs
url: /de/net/aspose.cells.pivot/pivottable/gethorizontalpagebreaks/
---
## PivotTable.GetHorizontalPageBreaks method

Ruft horizontale Seitenumbrüche dieser PivotTable ab.

```csharp
public int[] GetHorizontalPageBreaks()
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodGetHorizontalPageBreaksDemo
    {
        public static void Run()
        {
            // Ein Arbeitsbuch aus einer Quelldatei erstellen
            Workbook workbook = new Workbook("pivot_pagebreaks.xlsx");
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Greifen Sie auf die erste Pivot-Tabelle zu.
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // Pivot-Tabellendaten aktualisieren und berechnen
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Horizontale Seitenumbrüche abrufen
            int[] pageBreaks = pivotTable.GetHorizontalPageBreaks();
            
            // Ergebnisse anzeigen
            Console.WriteLine("Horizontal Page Breaks:");
            foreach (int row in pageBreaks)
            {
                Console.WriteLine("Row: " + row);
            }
        }
    }
}
```

### Siehe auch

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


