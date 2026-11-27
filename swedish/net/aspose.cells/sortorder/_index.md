---
title: "Enum SortOrder"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.SortOrder enum. Representerar sorteringsordning för dataområdet"
type: docs
url: /sv/net/aspose.cells/sortorder/
---
## SortOrder enumeration

Representerar sorteringsordning för dataområdet.

```csharp
public enum SortOrder
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Ascending | `0` | Sorterar data i stigande ordning |
| Descending | `1` | Sorterar data i fallande ordning |
| Natural | `2` | Behåller den ursprungliga dataordningen utan sortering. Gäller endast vissa speciella scenarier som PivotTable. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassSortOrderDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            var workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata för sortering
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Score");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(85);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(92);
            worksheet.Cells["A4"].PutValue("Bob");
            worksheet.Cells["B4"].PutValue(78);
            
            // Skapa datasortering
            var sorter = workbook.DataSorter;
            
            // Ange sorteringsordning och nycklar
            sorter.Order1 = SortOrder.Descending;
            sorter.Key1 = 1; // Sort by column B (Score)
            
            // Definiera sorteringsområde
            var sortArea = new CellArea
            {
                StartRow = 0,
                StartColumn = 0,
                EndRow = 3,
                EndColumn = 1
            };
            
            // Utför sorteringen
            sorter.Sort(worksheet.Cells, sortArea);
            
            // Spara arbetsboken
            workbook.Save("SortedData.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


