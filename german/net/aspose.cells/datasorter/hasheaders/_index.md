---
title: "DataSorter.HasHeaders"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DataSorter-Eigenschaft. Gibt an, ob der Bereich Überschriften enthält"
type: docs
url: /de/net/aspose.cells/datasorter/hasheaders/
---
## DataSorter.HasHeaders property

Gibt an, ob der Bereich Überschriften enthält.

```csharp
public bool HasHeaders { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterPropertyHasHeadersDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Kopfzeilen und Beispieldaten hinzufügen
            worksheet.Cells["A1"].PutValue("Fruits");
            worksheet.Cells["B1"].PutValue("Quantity");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["B2"].PutValue(15);
            worksheet.Cells["B3"].PutValue(8);
            worksheet.Cells["B4"].PutValue(12);

            // Daten‑Sorter erstellen und HasHeaders auf true setzen
            DataSorter sorter = workbook.DataSorter;
            sorter.HasHeaders = true; // This tells the sorter the first row contains headers
            
            // Nach der ersten Spalte (Fruits) in aufsteigender Reihenfolge sortieren
            sorter.AddKey(0, SortOrder.Ascending);
            
            // Den Datenbereich (einschließlich Kopfzeilen) sortieren
            sorter.Sort(worksheet.Cells, CellArea.CreateCellArea("A1", "B4"));

            // Die sortierte Arbeitsmappe speichern
            workbook.Save("SortedWithHeaders.xlsx");
        }
    }
}
```

### Siehe auch

* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


