---
title: "DataSorterKey.Color"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DataSorterKey-Eigenschaft. Gibt die sortierte Farbe zurück"
type: docs
url: /de/net/aspose.cells/datasorterkey/color/
---
## DataSorterKey.Color property

Liest die sortierte Farbe.

```csharp
public Color Color { get; }
```

### Hinweise

Wirkt nur, wenn [`Type`](../type/) CellColor oder FontColor ist.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class DataSorterKeyPropertyColorDemo
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

            // Geben Sie die Farbeigenschaft aus den Schlüsseln aus
            foreach (DataSorterKey k in sorter.Keys)
            {
                Console.WriteLine($"Color: {k.Color}");
            }
        }
    }
}
```

### Siehe auch

* class [DataSorterKey](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


