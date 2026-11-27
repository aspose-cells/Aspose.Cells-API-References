---
title: "DataSorter.Key3"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DataSorter egenskap. Representerar tredje sorterade kolumnindex (absolut position, kolumn A är 0, B är 1)"
type: docs
url: /sv/net/aspose.cells/datasorter/key3/
---
## DataSorter.Key3 property

Representerar tredje sorterade kolumnens index (absolut position, kolumn A är 0, B är 1, ...).

```csharp
public int Key3 { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterPropertyKey3Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Lägg till exempeldata
            cells["A1"].PutValue("Name");
            cells["B1"].PutValue("Score");
            cells["C1"].PutValue("Grade");
            cells["A2"].PutValue("John");
            cells["B2"].PutValue(85);
            cells["C2"].PutValue("B");
            cells["A3"].PutValue("Alice");
            cells["B3"].PutValue(92);
            cells["C3"].PutValue("A");
            cells["A4"].PutValue("Bob");
            cells["B4"].PutValue(78);
            cells["C4"].PutValue("C");
            cells["A5"].PutValue("Eve");
            cells["B5"].PutValue(92);
            cells["C5"].PutValue("A");

            // Skapa datasortering
            DataSorter sorter = workbook.DataSorter;
            
            // Sortera efter Poäng (fallande), sedan efter Namn (stigande), sedan efter Betyg (fallande)
            sorter.Order1 = SortOrder.Descending;
            sorter.Key1 = 1; // Column B (Score)
            
            sorter.Order2 = SortOrder.Ascending;
            sorter.Key2 = 0; // Column A (Name)
            
            sorter.Order3 = SortOrder.Descending;
            sorter.Key3 = 2; // Column C (Grade)
            
            // Sortera dataområde
            sorter.Sort(cells, CellArea.CreateCellArea(0, 0, 5, 2));

            // Spara arbetsboken
            workbook.Save("SortedData.xlsx");
        }
    }
}
```

### Se även

* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


