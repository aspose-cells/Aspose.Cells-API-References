---
title: "Enum SortOrder"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.SortOrder enum. Stellt die Sortierreihenfolge für den Datenbereich dar."
type: docs
url: /de/net/aspose.cells/sortorder/
---
## SortOrder enumeration

Stellt die Sortierreihenfolge für den Datenbereich dar.

```csharp
public enum SortOrder
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Ascending | `0` | Sortiert Daten in aufsteigender Reihenfolge |
| Descending | `1` | Sortiert Daten in absteigender Reihenfolge |
| Natural | `2` | Behält die ursprüngliche Datenreihenfolge bei, ohne zu sortieren. Gilt nur für einige spezielle Szenarien wie PivotTable. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassSortOrderDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            var workbook = new Workbook();
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Beispieldaten zum Sortieren hinzufügen
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Score");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(85);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(92);
            worksheet.Cells["A4"].PutValue("Bob");
            worksheet.Cells["B4"].PutValue(78);
            
            // Daten-Sortierer erstellen
            var sorter = workbook.DataSorter;
            
            // Sortierreihenfolge und Schlüssel festlegen
            sorter.Order1 = SortOrder.Descending;
            sorter.Key1 = 1; // Sort by column B (Score)
            
            // Sortierbereich definieren
            var sortArea = new CellArea
            {
                StartRow = 0,
                StartColumn = 0,
                EndRow = 3,
                EndColumn = 1
            };
            
            // Führe die Sortierung aus.
            sorter.Sort(worksheet.Cells, sortArea);
            
            // Speichere die Arbeitsmappe
            workbook.Save("SortedData.xlsx");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


