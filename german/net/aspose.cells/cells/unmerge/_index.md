---
title: "Cells.UnMerge"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cells-Methode. Hebt die Zusammenführung eines angegebenen Bereichs zusammengeführter Zellen auf"
type: docs
url: /de/net/aspose.cells/cells/unmerge/
---
## Cells.UnMerge method

Löst einen angegebenen Bereich zusammengeführter Zellen auf.

```csharp
public void UnMerge(int firstRow, int firstColumn, int totalRows, int totalColumns)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| firstRow | Int32 | Erste Zeile dieses Bereichs (nullbasiert) |
| firstColumn | Int32 | Erste Spalte dieses Bereichs (nullbasiert) |
| totalRows | Int32 | Anzahl der Zeilen (einsbasiert) |
| totalColumns | Int32 | Anzahl der Spalten (einsbasiert) |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodUnMergeWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Zellen zuerst zusammenführen
            cells.Merge(0, 0, 2, 2);
            
            // Die zuvor zusammengeführten Zellen wieder aufteilen
            cells.UnMerge(0, 0, 2, 2);
            
            // Speichere die Arbeitsmappe
            workbook.Save("UnMergeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


