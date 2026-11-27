---
title: "AdvancedFilter.ListRange"
second_title: "Aspose.Cells för .NET API‑referens"
description: "AdvancedFilter-egenskap. Hämtar listområdet för detta avancerade filter"
type: docs
url: /sv/net/aspose.cells/advancedfilter/listrange/
---
## AdvancedFilter.ListRange property

Hämtar listområdet för detta avancerade filter.

```csharp
public string ListRange { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AdvancedFilterPropertyListRangeDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Fyll i exempeldata
            sheet.Cells["A1"].PutValue("Name");
            sheet.Cells["B1"].PutValue("Age");
            for (int i = 2; i <= 10; i++)
            {
                sheet.Cells["A" + i].PutValue("Person " + (i-1));
                sheet.Cells["B" + i].PutValue(20 + i);
            }

            // Ställ in avancerat filter
            AdvancedFilter filter = sheet.GetAdvancedFilter();
            // ListRange är skrivskyddad och sätts automatiskt när filtret skapas
            // Vi kan bara läsa den, inte sätta den direkt
            
            // Visa listområdet (kommer att visa det automatiskt bestämda området)
            Console.WriteLine("Advanced Filter List Range: " + filter.ListRange);
            
            // Spara arbetsboken
            workbook.Save("AdvancedFilterDemo.xlsx");
        }
    }
}
```

### Se även

* class [AdvancedFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


