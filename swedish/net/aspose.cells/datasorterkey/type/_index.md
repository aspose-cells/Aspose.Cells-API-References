---
title: "DataSorterKey.Type"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DataSorterKey-egenskap. Representerar sorteringstypen"
type: docs
url: /sv/net/aspose.cells/datasorterkey/type/
---
## DataSorterKey.Type property

Representerar sorteringstypen.

```csharp
public SortOnType Type { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterKeyPropertyTypeDemo
    {
        public static void Run()
        {
            // Skapa ett arbetsbok-objekt
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("USA");
            worksheet.Cells["A2"].PutValue("China");
            worksheet.Cells["A3"].PutValue("Brazil");
            worksheet.Cells["A4"].PutValue("Russia");
            worksheet.Cells["A5"].PutValue("Canada");

            // Skapa datasortering och lägg till nyckel
            DataSorter sorter = workbook.DataSorter;
            sorter.AddKey(0, SortOrder.Ascending);

            // Sortera data
            CellArea ca = CellArea.CreateCellArea("A1", "A5");
            sorter.Sort(worksheet.Cells, ca);

            // Demonstrera användning av Type-egenskapen
            foreach (DataSorterKey key in sorter.Keys)
            {
                Console.WriteLine($"Key Type: {key.Type}");
            }
        }
    }
}
```

### Se även

* enum [SortOnType](../../sortontype/)
* class [DataSorterKey](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


