---
title: "Top10Filter.IsPercent"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Top10Filter-egenskap. Anger om filtrering ska ske efter procentvärdet i kolumnen"
type: docs
url: /sv/net/aspose.cells/top10filter/ispercent/
---
## Top10Filter.IsPercent property

Anger om du ska filtrera efter procentvärdet för kolumnen eller inte

```csharp
public bool IsPercent { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class Top10FilterPropertyIsPercentDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            for (int i = 0; i < 10; i++)
            {
                for (int j = 0; j < 10; j++)
                {
                    worksheet.Cells[i, j].PutValue((i + 1) * (j + 1));
                }
            }

            // Tillämpa top 10-filter (ej procent)
            worksheet.AutoFilter.Range = "A1:J10";
            worksheet.AutoFilter.FilterTop10(0, true, false, 5);
            
            // Hämta filtret och demonstrera IsPercent-egenskapen
            Top10Filter filter = worksheet.AutoFilter.FilterColumns[0].Filter as Top10Filter;
            Console.WriteLine("IsTop: " + filter.IsTop);
            Console.WriteLine("IsPercent: " + filter.IsPercent); // Should output False

            // Tillämpa top 10-procentfilter
            worksheet.AutoFilter.FilterTop10(1, true, true, 20);
            filter = worksheet.AutoFilter.FilterColumns[1].Filter as Top10Filter;
            Console.WriteLine("IsPercent: " + filter.IsPercent); // Should output True
        }
    }
}
```

### Se även

* class [Top10Filter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


