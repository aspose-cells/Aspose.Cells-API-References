---
title: "DataSorter.Order1"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DataSorter-Eigenschaft. Stellt die Sortierreihenfolge des ersten Schlüssels dar"
type: docs
url: /de/net/aspose.cells/datasorter/order1/
---
## DataSorter.Order1 property

Gibt die Sortierreihenfolge des ersten Schlüssels an.

```csharp
public SortOrder Order1 { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterPropertyOrder1Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Score");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(85);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(92);
            worksheet.Cells["A4"].PutValue("Bob");
            worksheet.Cells["B4"].PutValue(78);

            // Daten‑Sortierer‑Eigenschaften festlegen
            DataSorter sorter = workbook.DataSorter;
            sorter.Order1 = SortOrder.Ascending;
            sorter.Key1 = 1; // Sort by column B (Score)
            
            // Sortierbereich definieren
            CellArea area = CellArea.CreateCellArea("A1", "B4");
            
            // Führe die Sortierung aus.
            sorter.Sort(worksheet.Cells, area);
            
            // Speichere die Arbeitsmappe
            workbook.Save("SortedOutput.xlsx");
        }
    }
}
```

### Siehe auch

* enum [SortOrder](../../sortorder/)
* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


