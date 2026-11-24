---
title: "DataSorter.SortAsNumber"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DataSorter‑Eigenschaft. Gibt an, ob alles, was wie eine Zahl aussieht, sortiert wird"
type: docs
url: /de/net/aspose.cells/datasorter/sortasnumber/
---
## DataSorter.SortAsNumber property

Gibt an, ob alles, was wie eine Zahl aussieht, sortiert wird.

```csharp
public bool SortAsNumber { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterPropertySortAsNumberDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten mit gemischten Zahlen und Textzahlen hinzufügen
            worksheet.Cells["A1"].PutValue("Number");
            worksheet.Cells["A2"].PutValue("2");
            worksheet.Cells["A3"].PutValue("10");
            worksheet.Cells["A4"].PutValue("1");

            // Zellbereich zum Sortieren erstellen
            CellArea ca = CellArea.CreateCellArea("A1", "A4");

            // Daten-Sortierer erstellen
            DataSorter sorter = workbook.DataSorter;
            int idx = CellsHelper.ColumnNameToIndex("A");

            // Sortierschlüssel hinzufügen (Spalte A)
            sorter.AddKey(idx, SortOrder.Ascending);

            // Als Zahlen sortieren (true) oder als Zeichenketten (false)
            sorter.SortAsNumber = true;
            sorter.Sort(worksheet.Cells, ca);

            Console.WriteLine("Sorted as numbers:");
            for (int i = 1; i <= 4; i++)
            {
                Console.WriteLine(worksheet.Cells["A" + i].StringValue);
            }

            // Daten für die zweite Sortierung zurücksetzen
            worksheet.Cells["A2"].PutValue("2");
            worksheet.Cells["A3"].PutValue("10");
            worksheet.Cells["A4"].PutValue("1");

            // Als Zeichenketten sortieren
            sorter.SortAsNumber = false;
            sorter.Sort(worksheet.Cells, ca);

            Console.WriteLine("\nSorted as strings:");
            for (int i = 1; i <= 4; i++)
            {
                Console.WriteLine(worksheet.Cells["A" + i].StringValue);
            }
        }
    }
}
```

### Siehe auch

* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


