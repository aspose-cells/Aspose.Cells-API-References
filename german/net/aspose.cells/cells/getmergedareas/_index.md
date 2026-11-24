---
title: "Cells.GetMergedAreas"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cells-Methode. Ruft alle zusammengeführten Zellen ab"
type: docs
url: /de/net/aspose.cells/cells/getmergedareas/
---
## Cells.GetMergedAreas method

Gibt alle zusammengeführten Zellen zurück.

```csharp
public CellArea[] GetMergedAreas()
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGetMergedAreasDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Erstelle einige zusammengeführte Zellen
            worksheet.Cells.Merge(0, 0, 2, 2); // Merge A1:B2
            worksheet.Cells.Merge(3, 3, 3, 2); // Merge D4:E4
            worksheet.Cells.Merge(5, 0, 1, 5); // Merge A6:E6
            
            // Alle zusammengeführten Bereiche abrufen
            CellArea[] mergedAreas = worksheet.Cells.GetMergedAreas();
            
            // Informationen über zusammengeführte Bereiche anzeigen
            Console.WriteLine("Number of merged areas: " + mergedAreas.Length);
            foreach (CellArea area in mergedAreas)
            {
                Console.WriteLine($"Merged area: StartRow={area.StartRow}, StartColumn={area.StartColumn}, " +
                    $"EndRow={area.EndRow}, EndColumn={area.EndColumn}");
            }
        }
    }
}
```

### Siehe auch

* struct [CellArea](../../cellarea/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


