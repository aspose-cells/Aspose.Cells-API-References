---
title: "DataSorter.Key1"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DataSorter-egenskapen. Representerar första sorterade kolumnindexets absoluta position; kolumn A är 0, B är 1"
type: docs
url: /sv/net/aspose.cells/datasorter/key1/
---
## DataSorter.Key1 property

Representerar första sorterade kolumnens index (absolut position, kolumn A är 0, B är 1, ...).

```csharp
public int Key1 { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterPropertyKey1Demo
    {
        public static void Run()
        {
            // Skapa en arbetsbok och lägg till exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Lägg till exempeldata
            cells["A1"].PutValue("Name");
            cells["B1"].PutValue("Score");
            cells["A2"].PutValue("John");
            cells["B2"].PutValue(85);
            cells["A3"].PutValue("Alice");
            cells["B3"].PutValue(92);
            cells["A4"].PutValue("Bob");
            cells["B4"].PutValue(78);

            // Skapa en DataSorter och sätt Key1 för att sortera efter Score-kolumnen (kolumn B)
            DataSorter sorter = workbook.DataSorter;
            sorter.Key1 = 1; // Column index 1 (B)
            sorter.Order1 = SortOrder.Descending;

            // Definiera sorteringsområde (rader 1-4, alla datakolumner)
            CellArea sortArea = new CellArea();
            sortArea.StartRow = 1;
            sortArea.EndRow = 4;
            sortArea.StartColumn = 0;
            sortArea.EndColumn = cells.MaxDataColumn;

            // Utför sorteringen
            sorter.Sort(cells, sortArea);

            // Spara resultatet
            workbook.Save("SortedData.xlsx");
        }
    }
}
```

### Se även

* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


