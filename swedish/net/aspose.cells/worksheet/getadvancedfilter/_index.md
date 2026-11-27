---
title: "Worksheet.GetAdvancedFilter"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Worksheet-metod. Hämtar inställningarna för avancerat filter"
type: docs
url: /sv/net/aspose.cells/worksheet/getadvancedfilter/
---
## Worksheet.GetAdvancedFilter method

Hämtar inställningarna för avancerat filter.

```csharp
public AdvancedFilter GetAdvancedFilter()
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodGetAdvancedFilterDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Ställ in data för filtrering
            sheet.Cells["A1"].PutValue("Name");
            sheet.Cells["A2"].PutValue("John");
            sheet.Cells["A3"].PutValue("Alice");
            sheet.Cells["A4"].PutValue("Bob");
            
            // Ställ in kriterieintervall
            sheet.Cells["C1"].PutValue("Name");
            sheet.Cells["C2"].PutValue("John");
            
            // Applicera avancerat filter
            sheet.AdvancedFilter(true, "A1:A4", "C1:C2", "E1", false);
            
            // Hämta det avancerade filtret
            AdvancedFilter filter = sheet.GetAdvancedFilter();
            
            // Utdatafilterområden
            Console.WriteLine("List Range: " + filter.ListRange);
            Console.WriteLine("Criteria Range: " + filter.CriteriaRange);
            Console.WriteLine("Copy To Range: " + filter.CopyToRange);
        }
    }
}
```

### Se även

* class [AdvancedFilter](../../advancedfilter/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


