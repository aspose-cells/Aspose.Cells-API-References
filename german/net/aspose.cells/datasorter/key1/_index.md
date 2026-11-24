---
title: "DataSorter.Key1"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DataSorter‑Eigenschaft. Gibt den ersten sortierten Spaltenindex an; absolute Position: Spalte A ist 0, B ist 1"
type: docs
url: /de/net/aspose.cells/datasorter/key1/
---
## DataSorter.Key1 property

Gibt den Index der zuerst sortierten Spalte an (absolute Position, Spalte A ist 0, B ist 1, ...).

```csharp
public int Key1 { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterPropertyKey1Demo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe und füge Beispieldaten hinzu
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Fügen Sie Beispieldaten hinzu
            cells["A1"].PutValue("Name");
            cells["B1"].PutValue("Score");
            cells["A2"].PutValue("John");
            cells["B2"].PutValue(85);
            cells["A3"].PutValue("Alice");
            cells["B3"].PutValue(92);
            cells["A4"].PutValue("Bob");
            cells["B4"].PutValue(78);

            // Erstelle DataSorter und setze Key1, um nach der Score‑Spalte (Spalte B) zu sortieren
            DataSorter sorter = workbook.DataSorter;
            sorter.Key1 = 1; // Column index 1 (B)
            sorter.Order1 = SortOrder.Descending;

            // Definiere Sortierbereich (Zeilen 1‑4, alle Datenspalten)
            CellArea sortArea = new CellArea();
            sortArea.StartRow = 1;
            sortArea.EndRow = 4;
            sortArea.StartColumn = 0;
            sortArea.EndColumn = cells.MaxDataColumn;

            // Führe die Sortierung aus.
            sorter.Sort(cells, sortArea);

            // Ergebnis speichern
            workbook.Save("SortedData.xlsx");
        }
    }
}
```

### Siehe auch

* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


