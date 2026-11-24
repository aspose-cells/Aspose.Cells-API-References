---
title: "DataSorterKey.Index"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DataSorterKey-Eigenschaft. Gibt den sortierten Spaltenindex zurück, absolute Position, Spalte A ist 0, B ist 1"
type: docs
url: /de/net/aspose.cells/datasorterkey/index/
---
## DataSorterKey.Index property

Liest den sortierten Spaltenindex (absolute Position, Spalte A ist 0, B ist 1, ...).

```csharp
public int Index { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterKeyPropertyIndexDemo
    {
        public static void Run()
        {
            // Ein Arbeitsmappenobjekt erstellen
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten zum Sortieren hinzufügen
            worksheet.Cells["A1"].PutValue("USA");
            worksheet.Cells["A2"].PutValue("China");
            worksheet.Cells["A3"].PutValue("Brazil");
            worksheet.Cells["A4"].PutValue("Russia");
            worksheet.Cells["A5"].PutValue("Canada");

            // DataSorter erstellen und Sortierschlüssel hinzufügen
            DataSorter sorter = workbook.DataSorter;
            sorter.AddKey(0, SortOrder.Ascending);

            // Daten sortieren
            CellArea ca = CellArea.CreateCellArea("A1", "A5");
            sorter.Sort(worksheet.Cells, ca);

            // Verwendung der Index-Eigenschaft demonstrieren
            foreach (DataSorterKey key in sorter.Keys)
            {
                Console.WriteLine($"Column index being sorted: {key.Index}");
            }

            // Ergebnis speichern
            workbook.Save("DataSorterKeyExample.xlsx");
        }
    }
}
```

### Siehe auch

* class [DataSorterKey](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


