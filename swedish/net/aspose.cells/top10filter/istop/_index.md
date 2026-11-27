---
title: "Top10Filter.IsTop"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Top10Filter-egenskap. Anger om man ska filtrera efter toppordning eller inte"
type: docs
url: /sv/net/aspose.cells/top10filter/istop/
---
## Top10Filter.IsTop property

Anger om du ska filtrera efter översta ordning eller inte

```csharp
public bool IsTop { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class Top10FilterPropertyIsTopDemo
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
            }

            // Tillämpa topp 5-filter
            worksheet.AutoFilter.Range = "B6:B16";
            worksheet.AutoFilter.FilterTop10(0, true, false, 5);
            
            // Hämta filtret och kontrollera egenskapen IsTop
            Top10Filter filter = worksheet.AutoFilter.FilterColumns[0].Filter as Top10Filter;
            Console.WriteLine("IsTop: " + filter.IsTop); // Should output "True"
            Console.WriteLine("IsPercent: " + filter.IsPercent); // Should output "False"
            
            // Uppdatera filtret och kontrollera dolda rader
            worksheet.AutoFilter.Refresh();
            for (int i = 6; i <= 16; i++)
            {
                Console.WriteLine($"Row {i} hidden: {worksheet.Cells.IsRowHidden(i)}");
            }
        }
    }
}
```

### Se även

* class [Top10Filter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


