---
title: "DataSorterKey.Index"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DataSorterKey-egenskap. Hämtar det sorterade kolumnindexet, absolut position: kolumn A är 0, B är 1"
type: docs
url: /sv/net/aspose.cells/datasorterkey/index/
---
## DataSorterKey.Index property

Hämtar det sorterade kolumnindexet (absolut position, kolumn A är 0, B är 1, ...).

```csharp
public int Index { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterKeyPropertyIndexDemo
    {
        public static void Run()
        {
            // Skapa ett arbetsbok-objekt
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för sortering
            worksheet.Cells["A1"].PutValue("USA");
            worksheet.Cells["A2"].PutValue("China");
            worksheet.Cells["A3"].PutValue("Brazil");
            worksheet.Cells["A4"].PutValue("Russia");
            worksheet.Cells["A5"].PutValue("Canada");

            // Skapa datasortering och lägg till sorteringsnyckel
            DataSorter sorter = workbook.DataSorter;
            sorter.AddKey(0, SortOrder.Ascending);

            // Sortera data
            CellArea ca = CellArea.CreateCellArea("A1", "A5");
            sorter.Sort(worksheet.Cells, ca);

            // Demonstrera användning av Index-egenskapen
            foreach (DataSorterKey key in sorter.Keys)
            {
                Console.WriteLine($"Column index being sorted: {key.Index}");
            }

            // Spara resultatet
            workbook.Save("DataSorterKeyExample.xlsx");
        }
    }
}
```

### Se även

* class [DataSorterKey](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


