---
title: "PivotFilter.GetTop10Value"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotFilter-Methode. Gibt die Top‑10‑Einstellung des Filters zurück"
type: docs
url: /de/net/aspose.cells.pivot/pivotfilter/gettop10value/
---
## PivotFilter.GetTop10Value method

Ermittelt die Top‑10‑Einstellung des Filters.

```csharp
public Top10Filter GetTop10Value()
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFilterMethodGetTop10ValueDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe aus einer Quell‑Excel‑Datei
            Workbook workbook = new Workbook("example.xlsx");
            
            // Zugriff auf das erste Arbeitsblatt und die Pivot-Tabelle
            Worksheet worksheet = workbook.Worksheets[0];
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // Wenden Sie den Top‑10‑Filter auf das erste Basisfeld an (zeigen Sie die Top‑2‑Elemente nach Zählung)
            pivotTable.BaseFields[0].FilterTop10(0, PivotFilterType.Count, false, 2);
            
            // Rufen Sie den angewendeten Filter und dessen Top‑10‑Wert ab
            PivotFilter filter = pivotTable.BaseFields[0].GetFilters()[0];
            Top10Filter top10Filter = filter.GetTop10Value();
            
            // Geben Sie die Filterdetails aus
            Console.WriteLine("Filter Type: " + filter.FilterType);
            Console.WriteLine("Top 10 Items: " + top10Filter.Items);
            
            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [Top10Filter](../../../aspose.cells/top10filter/)
* class [PivotFilter](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


