---
title: "Klass Top10Filter"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Top10Filter-klass. Representerar de översta N procent eller antalet objekt att filtrera efter"
type: docs
url: /sv/net/aspose.cells/top10filter/
---
## Top10Filter class

Representerar de översta N (procent eller antal objekt) att filtrera efter.

```csharp
public class Top10Filter
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Criteria](../../aspose.cells/top10filter/criteria/) { get; set; } | (**Obsolete.**) Det faktiska cellvärdet i intervallet som används för att utföra jämförelsen för detta filter. Detta är cachevärdet under uppdateringsprocessen. |
| [IsPercent](../../aspose.cells/top10filter/ispercent/) { get; set; } | Anger om du ska filtrera efter procentvärdet för kolumnen eller inte |
| [IsTop](../../aspose.cells/top10filter/istop/) { get; set; } | Anger om du ska filtrera efter översta ordning eller inte |
| [Items](../../aspose.cells/top10filter/items/) { get; set; } | Hämtar och anger över- eller undervärde att använda som filterkriterium. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassTop10FilterDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata
            worksheet.Cells["B6"].PutValue("Value");
            for (int i = 7; i <= 16; i++)
            {
                worksheet.Cells["B" + i].PutValue(20 - i);
                worksheet.Cells["C" + i].PutValue("Item " + (i-6));
            }
            
            // Applicera autofilter och topp 10-filter
            worksheet.AutoFilter.Range = "B6:C16";
            worksheet.AutoFilter.FilterTop10(0, true, false, 5); // Filter top 5 values in column B
            
            // Hämta Top10Filter och verifiera dess egenskaper
            Top10Filter filter = worksheet.AutoFilter.FilterColumns[0].Filter as Top10Filter;
            Console.WriteLine("IsTop: " + filter.IsTop);
            Console.WriteLine("IsPercent: " + filter.IsPercent);
            Console.WriteLine("Items: " + filter.Items);
            
            // Uppdatera filtret och kontrollera dolda rader
            worksheet.AutoFilter.Refresh();
            for (int i = 6; i <= 16; i++)
            {
                Console.WriteLine($"Row {i} hidden: {worksheet.Cells.IsRowHidden(i)}");
            }
            
            // Spara arbetsboken
            workbook.Save("Top10FilterDemo.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


