---
title: "DataSorter.CaseSensitive"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DataSorter-egenskap. Hämtar och sätter om skiftlägeskänslig vid jämförelse av sträng"
type: docs
url: /sv/net/aspose.cells/datasorter/casesensitive/
---
## DataSorter.CaseSensitive property

Hämtar och anger om skiftlägeskänslighet vid jämförelse av sträng.

```csharp
public bool CaseSensitive { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterPropertyCaseSensitiveDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok och ett kalkylblad
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Lägg till exempeldata med skiftlägesvariationer
            cells["A1"].PutValue("apple");
            cells["A2"].PutValue("Orange");
            cells["A3"].PutValue("banana");
            cells["A4"].PutValue("APPLE");
            cells["A5"].PutValue("orange");
            cells["A6"].PutValue("Banana");

            // Skapa datasortering
            DataSorter sorter = workbook.DataSorter;
            sorter.Key1 = 0; // Sort by first column
            sorter.Order1 = SortOrder.Ascending;

            // Demonstrera skiftlägeskänslig sortering
            Console.WriteLine("Sorting with CaseSensitive = true:");
            sorter.CaseSensitive = true;
            sorter.Sort(cells, CellArea.CreateCellArea("A1", "A6"));
            PrintSortedData(cells, "A1:A6");

            // Demonstrera skiftlägesokänslig sortering
            Console.WriteLine("\nSorting with CaseSensitive = false:");
            sorter.CaseSensitive = false;
            sorter.Sort(cells, CellArea.CreateCellArea("A1", "A6"));
            PrintSortedData(cells, "A1:A6");
        }

        private static void PrintSortedData(Cells cells, string range)
        {
            Console.WriteLine("Sorted data:");
            foreach (Cell cell in cells.CreateRange(range))
            {
                Console.WriteLine(cell.StringValue);
            }
        }
    }
}
```

### Se även

* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


