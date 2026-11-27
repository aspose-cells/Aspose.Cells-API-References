---
title: "DataSorter.Order1"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DataSorter-egenskap. Representerar sorteringsordning för den första nyckeln"
type: docs
url: /sv/net/aspose.cells/datasorter/order1/
---
## DataSorter.Order1 property

Representerar sorteringsordning för den första nyckeln.

```csharp
public SortOrder Order1 { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterPropertyOrder1Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Score");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(85);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(92);
            worksheet.Cells["A4"].PutValue("Bob");
            worksheet.Cells["B4"].PutValue(78);

            // Ställ in egenskaper för datasortering
            DataSorter sorter = workbook.DataSorter;
            sorter.Order1 = SortOrder.Ascending;
            sorter.Key1 = 1; // Sort by column B (Score)
            
            // Definiera sorteringsintervall
            CellArea area = CellArea.CreateCellArea("A1", "B4");
            
            // Utför sorteringen
            sorter.Sort(worksheet.Cells, area);
            
            // Spara arbetsboken
            workbook.Save("SortedOutput.xlsx");
        }
    }
}
```

### Se även

* enum [SortOrder](../../sortorder/)
* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


