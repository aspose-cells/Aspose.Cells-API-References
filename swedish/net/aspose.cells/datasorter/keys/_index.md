---
title: "DataSorter.Keys"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DataSorter-egenskap. Hämtar nyckellistan för data sorter"
type: docs
url: /sv/net/aspose.cells/datasorter/keys/
---
## DataSorter.Keys property

Hämtar nyckellistan för data sorter.

```csharp
public DataSorterKeyCollection Keys { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterPropertyKeysDemo
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

            // Initiera data sorter
            DataSorter sorter = workbook.DataSorter;
            
            // Lägg till sorteringsnyckel för kolumn A (index 0)
            sorter.AddKey(0, SortOrder.Ascending);

            // Sortera data
            sorter.Sort(worksheet.Cells, CellArea.CreateCellArea("A1", "A5"));

            // Demonstrera användning av egenskapen Keys
            DataSorterKeyCollection keys = sorter.Keys;
            Console.WriteLine("Sort Keys Information:");
            foreach (DataSorterKey key in keys)
            {
                Console.WriteLine($"Column Index: {key.Index}, Sort Order: {key.Order}");
            }

            // Spara arbetsboken
            workbook.Save("DataSorterKeysDemo.xlsx");
        }
    }
}
```

### Se även

* class [DataSorterKeyCollection](../../datasorterkeycollection/)
* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


