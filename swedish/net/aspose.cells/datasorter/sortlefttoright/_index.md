---
title: "DataSorter.SortLeftToRight"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DataSorter-egenskapen. True betyder att sorteringsorienteringen är från vänster till höger. False betyder att sorteringsorienteringen är från topp till botten. Standardvärdet är false"
type: docs
url: /sv/net/aspose.cells/datasorter/sortlefttoright/
---
## DataSorter.SortLeftToRight property

Sant betyder att sorteringsriktningen är från vänster till höger. Falskt betyder att sorteringsriktningen är från topp till botten. Standardvärdet är falskt.

```csharp
public bool SortLeftToRight { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterPropertySortLeftToRightDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Exempeldatat (kolumner kommer att behandlas som rader när SortLeftToRight=true)
            worksheet.Cells["A1"].PutValue(3);
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B1"].PutValue("C");
            worksheet.Cells["B2"].PutValue("A");
            worksheet.Cells["B3"].PutValue("B");

            // Skapa en DataSorter och ställ in för att sortera från vänster till höger
            DataSorter sorter = workbook.DataSorter;
            sorter.SortLeftToRight = true;

            // Ange sorteringsnyckel (kolumnindex blir radindex när sortering sker från vänster till höger)
            sorter.Key1 = 0; // Sort by first "row" (originally column A)

            // Definiera sorteringsområde (rader blir kolumner när sortering sker från vänster till höger)
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 2;
            area.StartColumn = 0;
            area.EndColumn = 1;

            // Utför sorteringen
            sorter.Sort(worksheet.Cells, area);

            // Spara resultatet
            workbook.Save("SortedLeftToRight.xlsx");
        }
    }
}
```

### Se även

* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


