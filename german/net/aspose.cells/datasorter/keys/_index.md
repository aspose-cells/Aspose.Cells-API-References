---
title: "DataSorter.Keys"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DataSorter-Eigenschaft. Gibt die Schlüsselliste des DataSorters zurück"
type: docs
url: /de/net/aspose.cells/datasorter/keys/
---
## DataSorter.Keys property

Liefert die Schlüsselliste des DataSorters.

```csharp
public DataSorterKeyCollection Keys { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterPropertyKeysDemo
    {
        public static void Run()
        {
            // Ein Arbeitsmappenobjekt erstellen
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("USA");
            worksheet.Cells["A2"].PutValue("China");
            worksheet.Cells["A3"].PutValue("Brazil");
            worksheet.Cells["A4"].PutValue("Russia");
            worksheet.Cells["A5"].PutValue("Canada");

            // DataSorter initialisieren
            DataSorter sorter = workbook.DataSorter;
            
            // Sortierschlüssel für Spalte A (Index 0) hinzufügen
            sorter.AddKey(0, SortOrder.Ascending);

            // Daten sortieren
            sorter.Sort(worksheet.Cells, CellArea.CreateCellArea("A1", "A5"));

            // Verwendung der Keys-Eigenschaft demonstrieren
            DataSorterKeyCollection keys = sorter.Keys;
            Console.WriteLine("Sort Keys Information:");
            foreach (DataSorterKey key in keys)
            {
                Console.WriteLine($"Column Index: {key.Index}, Sort Order: {key.Order}");
            }

            // Speichere die Arbeitsmappe
            workbook.Save("DataSorterKeysDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [DataSorterKeyCollection](../../datasorterkeycollection/)
* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


