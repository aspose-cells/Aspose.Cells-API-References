---
title: "DataSorterKeyCollection.Item"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DataSorterKeyCollection-egenskap. Hämtar och anger DataSorterKey efter index"
type: docs
url: /sv/net/aspose.cells/datasorterkeycollection/item/
---
## DataSorterKeyCollection indexer

Hämtar och anger [`DataSorterKey`](../../datasorterkey/) efter index.

```csharp
public DataSorterKey this[int index] { get; }
```

| Parameter | Beskrivning |
| --- | --- |
| index | Indexet. |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class DataSorterKeyCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["A4"].PutValue("Bob");
            worksheet.Cells["B1"].PutValue("Score");
            worksheet.Cells["B2"].PutValue(85);
            worksheet.Cells["B3"].PutValue(92);
            worksheet.Cells["B4"].PutValue(78);

            // Skapa ett listobjekt (tabell)
            int index = worksheet.ListObjects.Add(0, 0, 3, 1, true);
            ListObject table = worksheet.ListObjects[index];

            // Lägg till sorteringsnyckel (sortera efter Score-kolumnen i fallande ordning)
            table.AutoFilter.Sorter.AddKey(1, SortOrder.Descending);
            table.AutoFilter.Sorter.Sort();

            // Demonstrera användning av Item-egenskapen
            DataSorterKey key = table.AutoFilter.Sorter.Keys[0];
            Console.WriteLine("Sort Key Index: {0}, Order: {1}", key.Index, key.Order);

            // Spara arbetsboken
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [DataSorterKey](../../datasorterkey/)
* class [DataSorterKeyCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


