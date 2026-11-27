---
title: "FilterColumn.CustomFilters"
second_title: "Aspose.Cells för .NET API‑referens"
description: "FilterColumn egenskap. Hämtar CustomFilterCollection för filtrering av data efter anpassade kriterier"
type: docs
url: /sv/net/aspose.cells/filtercolumn/customfilters/
---
## FilterColumn.CustomFilters property

Hämtar [`CustomFilterCollection`](../../customfiltercollection/) för filtrering av data efter anpassade kriterier.

```csharp
public CustomFilterCollection CustomFilters { get; set; }
```

### Anmärkningar

OBS: Denna setter för denna egenskap är nu föråldrad. Använd istället egenskapen [`FilterType`](../filtertype/) genom att sätta den till CustomFilters. Denna egenskap kommer att tas bort 12 månader senare från och med juni 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FilterColumnPropertyCustomFiltersDemo
    {
        public static void Run()
        {
            try
            {
                // Skapa en ny arbetsbok
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Lägg till exempeldata
                worksheet.Cells["A1"].PutValue("Product");
                worksheet.Cells["A2"].PutValue("Apple");
                worksheet.Cells["A3"].PutValue("Banana");
                worksheet.Cells["A4"].PutValue("Cherry");
                worksheet.Cells["A5"].PutValue("Date");
                worksheet.Cells["A6"].PutValue("Elderberry");

                // Applicera autofilter
                worksheet.AutoFilter.Range = "A1:A6";

                // Hämta filterkolumnen
                FilterColumn filterColumn = worksheet.AutoFilter.FilterColumns[0];

                // Skapa och ställ in anpassade filter med metoden AutoFilter.Custom
                // Första filtret: börjar med "A"
                worksheet.AutoFilter.Custom(0, FilterOperatorType.BeginsWith, "A", false, FilterOperatorType.None, null);

                // Andra filtret: slutar med "y" (OCH-relation)
                worksheet.AutoFilter.Custom(0, FilterOperatorType.EndsWith, "y", true, FilterOperatorType.None, null);

                // Hämta de anpassade filtren från filterkolumnen
                CustomFilterCollection customFilters = filterColumn.CustomFilters;

                // Visa information om de anpassade filtren
                Console.WriteLine($"Number of custom filters: {customFilters.Count}");
                Console.WriteLine($"Filter relationship (And): {customFilters.And}");

                // Obs: CustomFilterCollection exponerar inte enskilda filter direkt
                // genom en indexerare, så vi kan bara visa samlingens egenskaper
                Console.WriteLine("Custom filters have been applied to the column.");

                // Spara arbetsboken
                workbook.Save("CustomFiltersDemo.xlsx");
                Console.WriteLine("CustomFilters demonstration completed successfully.");
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

* class [CustomFilterCollection](../../customfiltercollection/)
* class [FilterColumn](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


