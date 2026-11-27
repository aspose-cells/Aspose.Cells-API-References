---
title: "AdvancedFilter.CriteriaRange"
second_title: "Aspose.Cells för .NET API‑referens"
description: "AdvancedFilter-egenskap. Hämtar kriterieområdet för detta avancerade filter"
type: docs
url: /sv/net/aspose.cells/advancedfilter/criteriarange/
---
## AdvancedFilter.CriteriaRange property

Hämtar kriterieområdet för detta avancerade filter.

```csharp
public string CriteriaRange { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AdvancedFilterPropertyCriteriaRangeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok och hämta det första kalkylbladet
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Fyll i exempeldata för listområdet
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["B1"].PutValue("Amount");
            sheet.Cells["A2"].PutValue("Food");
            sheet.Cells["B2"].PutValue(120);
            sheet.Cells["A3"].PutValue("Transport");
            sheet.Cells["B3"].PutValue(80);
            sheet.Cells["A4"].PutValue("Food");
            sheet.Cells["B4"].PutValue(150);

            // Fyll i exempel på kriterier (filtret kommer att använda detta när det tillämpas)
            sheet.Cells["D1"].PutValue("Category");
            sheet.Cells["D2"].PutValue("Food");

            try
            {
                // Hämta AdvancedFilter-objektet för kalkylbladet
                AdvancedFilter filter = sheet.GetAdvancedFilter();

                // ListRange-, CriteriaRange- och CopyToRange‑egenskaperna är skrivskyddade.
                // Visa de automatiskt bestämda intervallen.
                Console.WriteLine("List Range:    " + filter.ListRange);
                Console.WriteLine("Criteria Range:" + filter.CriteriaRange);
                Console.WriteLine("Copy To Range: " + filter.CopyToRange);

                // Spara arbetsboken (valfritt, bara för att visa att filen kan skapas)
                workbook.Save("AdvancedFilterCriteriaRangeDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [AdvancedFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


