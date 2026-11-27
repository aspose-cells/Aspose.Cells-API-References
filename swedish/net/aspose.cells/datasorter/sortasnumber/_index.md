---
title: "DataSorter.SortAsNumber"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DataSorter egenskap. Anger om sortering av allt som ser ut som ett tal"
type: docs
url: /sv/net/aspose.cells/datasorter/sortasnumber/
---
## DataSorter.SortAsNumber property

Indikerar om sortering av allt som ser ut som ett tal.

```csharp
public bool SortAsNumber { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterPropertySortAsNumberDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata med blandade tal och texttal
            worksheet.Cells["A1"].PutValue("Number");
            worksheet.Cells["A2"].PutValue("2");
            worksheet.Cells["A3"].PutValue("10");
            worksheet.Cells["A4"].PutValue("1");

            // Skapa cellområde för sortering
            CellArea ca = CellArea.CreateCellArea("A1", "A4");

            // Skapa datasortering
            DataSorter sorter = workbook.DataSorter;
            int idx = CellsHelper.ColumnNameToIndex("A");

            // Lägg till sorteringsnyckel (kolumn A)
            sorter.AddKey(idx, SortOrder.Ascending);

            // Sortera som tal (true) eller strängar (false)
            sorter.SortAsNumber = true;
            sorter.Sort(worksheet.Cells, ca);

            Console.WriteLine("Sorted as numbers:");
            for (int i = 1; i <= 4; i++)
            {
                Console.WriteLine(worksheet.Cells["A" + i].StringValue);
            }

            // Återställ data för andra sorteringen
            worksheet.Cells["A2"].PutValue("2");
            worksheet.Cells["A3"].PutValue("10");
            worksheet.Cells["A4"].PutValue("1");

            // Sortera som strängar
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

### Se även

* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


