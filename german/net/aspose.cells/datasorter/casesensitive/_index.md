---
title: "DataSorter.CaseSensitive"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DataSorter‑Eigenschaft. Gibt an, ob bei Zeichenkettenvergleichen die Groß‑/Kleinschreibung beachtet wird, und legt sie fest"
type: docs
url: /de/net/aspose.cells/datasorter/casesensitive/
---
## DataSorter.CaseSensitive property

Liest und setzt, ob bei Zeichenkettenvergleich die Groß-/Kleinschreibung beachtet wird.

```csharp
public bool CaseSensitive { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterPropertyCaseSensitiveDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe und ein Arbeitsblatt
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Beispieldaten mit Groß‑/Kleinschreibungsvariationen hinzufügen
            cells["A1"].PutValue("apple");
            cells["A2"].PutValue("Orange");
            cells["A3"].PutValue("banana");
            cells["A4"].PutValue("APPLE");
            cells["A5"].PutValue("orange");
            cells["A6"].PutValue("Banana");

            // Daten-Sortierer erstellen
            DataSorter sorter = workbook.DataSorter;
            sorter.Key1 = 0; // Sort by first column
            sorter.Order1 = SortOrder.Ascending;

            // Sortierung mit Beachtung der Groß‑/Kleinschreibung demonstrieren
            Console.WriteLine("Sorting with CaseSensitive = true:");
            sorter.CaseSensitive = true;
            sorter.Sort(cells, CellArea.CreateCellArea("A1", "A6"));
            PrintSortedData(cells, "A1:A6");

            // Sortierung ohne Beachtung der Groß‑/Kleinschreibung demonstrieren
            Console.WriteLine("\nSorting with CaseSensitive = false:");
            sorter.CaseSensitive = false;
            sorter.Sort(cells, CellArea.CreateCellArea("A1", "A6"));
            PrintSortedData(cells, "A1:A6");
        }

        private static void PrintSortedData(Cells cells, string range)
        {
            Console.WriteLine("Sorted data:");
            foreach (Cell cell in cells.CreateRange(range))
            {
                Console.WriteLine(cell.StringValue);
            }
        }
    }
}
```

### Siehe auch

* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


