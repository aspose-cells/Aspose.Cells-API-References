---
title: "DataSorter.SortLeftToRight"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DataSorter‑Eigenschaft. True bedeutet, dass die Sortierrichtung von links nach rechts ist. False bedeutet, dass die Sortierrichtung von oben nach unten ist. Der Standardwert ist false"
type: docs
url: /de/net/aspose.cells/datasorter/sortlefttoright/
---
## DataSorter.SortLeftToRight property

True bedeutet, dass die Sortierrichtung von links nach rechts verläuft. False bedeutet, dass die Sortierrichtung von oben nach unten verläuft. Der Standardwert ist false.

```csharp
public bool SortLeftToRight { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterPropertySortLeftToRightDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten (Spalten werden als Zeilen behandelt, wenn SortLeftToRight=true)
            worksheet.Cells["A1"].PutValue(3);
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B1"].PutValue("C");
            worksheet.Cells["B2"].PutValue("A");
            worksheet.Cells["B3"].PutValue("B");

            // Erstelle DataSorter und setze ihn auf Sortierung von links nach rechts
            DataSorter sorter = workbook.DataSorter;
            sorter.SortLeftToRight = true;

            // Setze Sortierschlüssel (Spaltenindex wird zum Zeilenindex bei Sortierung von links nach rechts)
            sorter.Key1 = 0; // Sort by first "row" (originally column A)

            // Definiere Sortierbereich (Zeilen werden zu Spalten bei Sortierung von links nach rechts)
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 2;
            area.StartColumn = 0;
            area.EndColumn = 1;

            // Führe die Sortierung aus.
            sorter.Sort(worksheet.Cells, area);

            // Ergebnis speichern
            workbook.Save("SortedLeftToRight.xlsx");
        }
    }
}
```

### Siehe auch

* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


