---
title: "PivotFilter.FilterType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotFilter-Eigenschaft. Gibt den Filtertyp des Pivotfilters zurück"
type: docs
url: /de/net/aspose.cells.pivot/pivotfilter/filtertype/
---
## PivotFilter.FilterType property

Ermittelt den Filtertyp des Pivotfilters.

```csharp
public PivotFilterType FilterType { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFilterPropertyFilterTypeDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe aus einer Quell‑Excel‑Datei
            Workbook workbook = new Workbook("example.xlsx");
            
            // Zugriff auf das erste Arbeitsblatt und die Pivot-Tabelle
            Worksheet worksheet = workbook.Worksheets[0];
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // Wertfilter (kleiner als 2) auf das erste Basisfeld anwenden
            pivotTable.BaseFields[0].FilterByValue(0, PivotFilterType.ValueLessThan, 2, 0);
            
            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");
            
            // Arbeitsmappe neu laden, um den Filter zu überprüfen
            Workbook verifyWorkbook = new Workbook("output.xlsx");
            PivotTable verifyPivotTable = verifyWorkbook.Worksheets[0].PivotTables[0];
            
            // Den angewendeten Filter abrufen und die FilterType-Eigenschaft demonstrieren
            PivotFilter filter = verifyPivotTable.BaseFields[0].GetFilters()[0];
            Console.WriteLine("Filter Type: " + filter.FilterType); // Should output ValueLessThan
            Console.WriteLine("Filter Value: " + filter.GetNumberValues()[0]); // Should output 2
        }
    }
}
```

### Siehe auch

* enum [PivotFilterType](../../pivotfiltertype/)
* class [PivotFilter](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


