---
title: "DataSorterKey.Type"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DataSorterKey-Eigenschaft. Stellt den Typ der Sortierung dar"
type: docs
url: /de/net/aspose.cells/datasorterkey/type/
---
## DataSorterKey.Type property

Stellt den Sortierungstyp dar.

```csharp
public SortOnType Type { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterKeyPropertyTypeDemo
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

            // Erstellen Sie einen DataSorter und fügen Sie einen Schlüssel hinzu
            DataSorter sorter = workbook.DataSorter;
            sorter.AddKey(0, SortOrder.Ascending);

            // Daten sortieren
            CellArea ca = CellArea.CreateCellArea("A1", "A5");
            sorter.Sort(worksheet.Cells, ca);

            // Demonstriere die Verwendung der Type‑Eigenschaft
            foreach (DataSorterKey key in sorter.Keys)
            {
                Console.WriteLine($"Key Type: {key.Type}");
            }
        }
    }
}
```

### Siehe auch

* enum [SortOnType](../../sortontype/)
* class [DataSorterKey](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


