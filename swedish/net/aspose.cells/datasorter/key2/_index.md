---
title: "DataSorter.Key2"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DataSorter-egenskap. Representerar andra sorterade kolumnens index, absolut position kolumn A är 0 B är 1"
type: docs
url: /sv/net/aspose.cells/datasorter/key2/
---
## DataSorter.Key2 property

Representerar andra sorterade kolumnens index (absolut position, kolumn A är 0, B är 1, ...).

```csharp
public int Key2 { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterPropertyKey2Demo
    {
        public static void Run()
        {
            // Skapa en arbetsbok och lägg till exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);
            worksheet.Cells["A4"].PutValue("Bob");
            worksheet.Cells["B4"].PutValue(35);

            // Skapa DataSorter och sätt egenskaper
            DataSorter sorter = workbook.DataSorter;
            sorter.HasHeaders = true;
            sorter.Key1 = 0; // Sort by first column (Name)
            sorter.Order1 = SortOrder.Ascending;
            sorter.Key2 = 1; // Then sort by second column (Age)
            sorter.Order2 = SortOrder.Descending;

            // Sortera dataområde
            sorter.Sort(worksheet.Cells, 0, 0, 3, 1);

            // Skriv ut den sorterade datan för att demonstrera användning av Key2
            Console.WriteLine("Sorted Data:");
            for (int i = 0; i <= 3; i++)
            {
                Console.WriteLine($"{worksheet.Cells[i, 0].StringValue} - {worksheet.Cells[i, 1].IntValue}");
            }
        }
    }
}
```

### Se även

* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


