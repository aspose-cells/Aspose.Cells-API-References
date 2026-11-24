---
title: "DataSorter.Order3"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DataSorter‑Eigenschaft. Stellt die Sortierreihenfolge des dritten Schlüssels dar"
type: docs
url: /de/net/aspose.cells/datasorter/order3/
---
## DataSorter.Order3 property

Gibt die Sortierreihenfolge des dritten Schlüssels an.

```csharp
public SortOrder Order3 { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterPropertyOrder3Demo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe und füge Beispieldaten hinzu
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Beispieldaten zum Sortieren hinzufügen
            cells["A1"].PutValue("Department");
            cells["B1"].PutValue("Name");
            cells["C1"].PutValue("Salary");
            
            cells["A2"].PutValue("HR");
            cells["B2"].PutValue("John");
            cells["C2"].PutValue(5000);
            
            cells["A3"].PutValue("IT");
            cells["B3"].PutValue("Alice");
            cells["C3"].PutValue(6000);
            
            cells["A4"].PutValue("HR");
            cells["B4"].PutValue("Bob");
            cells["C4"].PutValue(4500);
            
            cells["A5"].PutValue("IT");
            cells["B5"].PutValue("Charlie");
            cells["C5"].PutValue(7000);

            // Daten‑Sorter erstellen und Sortierschlüssel sowie -reihenfolgen festlegen
            DataSorter sorter = workbook.DataSorter;
            sorter.Key1 = 0; // Sort by Department (column A)
            sorter.Order1 = SortOrder.Ascending;
            
            sorter.Key2 = 1; // Then by Name (column B)
            sorter.Order2 = SortOrder.Descending;
            
            sorter.Key3 = 2; // Finally by Salary (column C)
            sorter.Order3 = SortOrder.Ascending;
            
            sorter.CaseSensitive = false;

            // Den zu sortierenden Bereich definieren (Kopfzeilen + 4 Datenzeilen)
            CellArea range = new CellArea();
            range.StartRow = 0;
            range.StartColumn = 0;
            range.EndRow = 4;
            range.EndColumn = 2;

            // Führe die Sortierung aus.
            sorter.Sort(cells, range);

            // Die sortierten Daten ausgeben
            Console.WriteLine("Sorted Data:");
            for (int row = 0; row <= 4; row++)
            {
                Console.WriteLine($"{cells[row, 0].StringValue}, {cells[row, 1].StringValue}, {cells[row, 2].IntValue}");
            }
        }
    }
}
```

### Siehe auch

* enum [SortOrder](../../sortorder/)
* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


