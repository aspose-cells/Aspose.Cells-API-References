---
title: "DataSorter.HasHeaders"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DataSorter-egenskap. Representerar om intervallet har rubriker"
type: docs
url: /sv/net/aspose.cells/datasorter/hasheaders/
---
## DataSorter.HasHeaders property

Representerar om intervallet har rubriker.

```csharp
public bool HasHeaders { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterPropertyHasHeadersDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till rubriker och exempeldata
            worksheet.Cells["A1"].PutValue("Fruits");
            worksheet.Cells["B1"].PutValue("Quantity");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["B2"].PutValue(15);
            worksheet.Cells["B3"].PutValue(8);
            worksheet.Cells["B4"].PutValue(12);

            // Skapa data sorter och sätt HasHeaders till true
            DataSorter sorter = workbook.DataSorter;
            sorter.HasHeaders = true; // This tells the sorter the first row contains headers
            
            // Sortera efter den första kolumnen (Fruits) i stigande ordning
            sorter.AddKey(0, SortOrder.Ascending);
            
            // Sortera dataområdet (inklusive rubriker)
            sorter.Sort(worksheet.Cells, CellArea.CreateCellArea("A1", "B4"));

            // Spara den sorterade arbetsboken
            workbook.Save("SortedWithHeaders.xlsx");
        }
    }
}
```

### Se även

* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


