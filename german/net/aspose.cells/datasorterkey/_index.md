---
title: "Klasse DataSorterKey"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.DataSorterKey-Klasse. Stellt den Schlüssel des Datensortierers dar"
type: docs
url: /de/net/aspose.cells/datasorterkey/
---
## DataSorterKey class

Stellt den Schlüssel des DataSorters dar.

```csharp
public class DataSorterKey
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Color](../../aspose.cells/datasorterkey/color/) { get; } | Liest die sortierte Farbe. |
| [IconId](../../aspose.cells/datasorterkey/iconid/) { get; } | Stellt die ID des Symbolsatztyps dar. |
| [IconSetType](../../aspose.cells/datasorterkey/iconsettype/) { get; } | Stellt den Symbolsatztyp dar. |
| [Index](../../aspose.cells/datasorterkey/index/) { get; } | Liest den sortierten Spaltenindex (absolute Position, Spalte A ist 0, B ist 1, ...). |
| [Order](../../aspose.cells/datasorterkey/order/) { get; } | Gibt die Reihenfolge der Sortierung an. |
| [Type](../../aspose.cells/datasorterkey/type/) { get; } | Stellt den Sortierungstyp dar. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class DataSorterKeyDemo
    {
        public static void DataSorterKeyExample()
        {
            // Erstellen Sie ein Arbeitsmappen‑Objekt und laden Sie eine Vorlagendatei
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie einige Beispieldaten zum Sortieren hinzu
            worksheet.Cells["A1"].PutValue("USA");
            worksheet.Cells["A2"].PutValue("China");
            worksheet.Cells["A3"].PutValue("Brazil");
            worksheet.Cells["A4"].PutValue("Russia");
            worksheet.Cells["A5"].PutValue("Canada");

            // Instanziere Daten‑Sortierobjekt
            DataSorter sorter = workbook.DataSorter;

            // Füge Schlüssel für die erste Spalte (A) hinzu, um aufsteigend zu sortieren.
            sorter.AddKey(0, SortOrder.Ascending);

            // Erstelle einen Zellbereich (Range), der sortiert werden soll.
            CellArea ca = CellArea.CreateCellArea("A1", "A5");

            // Führe die Sortierung aus.
            sorter.Sort(worksheet.Cells, ca);

            // Speichere die Ausgabedatei.
            workbook.Save("DataSorterKeyExample.xlsx");
            workbook.Save("DataSorterKeyExample.pdf");

            // Greife auf die DataSorterKeyCollection zu
            DataSorterKeyCollection keys = sorter.Keys;

            // Iteriere über die Schlüssel und gib deren Eigenschaften aus.
            foreach (DataSorterKey key in keys)
            {
                Console.WriteLine($"Order: {key.Order}");
                Console.WriteLine($"Index: {key.Index}");
                Console.WriteLine($"Type: {key.Type}");
                Console.WriteLine($"IconSetType: {key.IconSetType}");
                Console.WriteLine($"IconId: {key.IconId}");
                Console.WriteLine($"Color: {key.Color}");
            }
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


