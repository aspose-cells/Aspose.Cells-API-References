---
title: "DataSorter.Key3"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DataSorter-Eigenschaft. Stellt den Index der dritten sortierten Spalte dar (absolute Position, Spalte A ist 0, B ist 1)"
type: docs
url: /de/net/aspose.cells/datasorter/key3/
---
## DataSorter.Key3 property

Gibt den Index der drittens sortierten Spalte an (absolute Position, Spalte A ist 0, B ist 1, ...).

```csharp
public int Key3 { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterPropertyKey3Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Fügen Sie Beispieldaten hinzu
            cells["A1"].PutValue("Name");
            cells["B1"].PutValue("Score");
            cells["C1"].PutValue("Grade");
            cells["A2"].PutValue("John");
            cells["B2"].PutValue(85);
            cells["C2"].PutValue("B");
            cells["A3"].PutValue("Alice");
            cells["B3"].PutValue(92);
            cells["C3"].PutValue("A");
            cells["A4"].PutValue("Bob");
            cells["B4"].PutValue(78);
            cells["C4"].PutValue("C");
            cells["A5"].PutValue("Eve");
            cells["B5"].PutValue(92);
            cells["C5"].PutValue("A");

            // Daten-Sortierer erstellen
            DataSorter sorter = workbook.DataSorter;
            
            // Nach Punktzahl sortieren (absteigend), dann nach Name (aufsteigend), dann nach Note (absteigend)
            sorter.Order1 = SortOrder.Descending;
            sorter.Key1 = 1; // Column B (Score)
            
            sorter.Order2 = SortOrder.Ascending;
            sorter.Key2 = 0; // Column A (Name)
            
            sorter.Order3 = SortOrder.Descending;
            sorter.Key3 = 2; // Column C (Grade)
            
            // Datenbereich sortieren
            sorter.Sort(cells, CellArea.CreateCellArea(0, 0, 5, 2));

            // Speichere die Arbeitsmappe
            workbook.Save("SortedData.xlsx");
        }
    }
}
```

### Siehe auch

* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


