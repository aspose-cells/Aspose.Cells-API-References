---
title: "FilterColumn.IconFilter"
second_title: "Aspose.Cells för .NET API‑referens"
description: "FilterColumn-egenskap. Hämtar IconFilter för att filtrera data efter ikon"
type: docs
url: /sv/net/aspose.cells/filtercolumn/iconfilter/
---
## FilterColumn.IconFilter property

Hämtar `IconFilter` för att filtrera data efter ikon.

```csharp
public IconFilter IconFilter { get; }
```

### Anmärkningar

Innan du använder den här egenskapen, se till att [`FilterType`](../filtertype/) är IconFilter, annars returneras null.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FilterColumnPropertyIconFilterDemo
    {
        public static void Run()
        {
            try
            {
                // Skapa en ny arbetsbok
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Lägg till exempeldata med villkorsstyrd formatering som använder ikoner
                worksheet.Cells["A1"].PutValue("Performance");
                worksheet.Cells["A2"].PutValue(85);
                worksheet.Cells["A3"].PutValue(72);
                worksheet.Cells["A4"].PutValue(93);
                worksheet.Cells["A5"].PutValue(65);

                // Applicera autofilter på intervallet
                worksheet.AutoFilter.Range = "A1:A5";

                // Hämta filterkolumnen
                FilterColumn filterColumn = worksheet.AutoFilter.FilterColumns[0];

                // Åtkomst till IconFilter-egenskapen (skrivskyddad)
                IconFilter iconFilter = filterColumn.IconFilter;

                // Visa IconFilter-egenskaper om den finns
                if (iconFilter != null)
                {
                    Console.WriteLine("IconFilter is available");
                    Console.WriteLine($"IconSetType: {iconFilter.IconSetType}");
                    Console.WriteLine($"IconId: {iconFilter.IconId}");
                }
                else
                {
                    Console.WriteLine("No IconFilter is currently applied to this column");
                }

                // Spara arbetsboken
                workbook.Save("IconFilterDemo.xlsx");
                Console.WriteLine("IconFilter demonstration completed successfully.");
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

* class [IconFilter](../../iconfilter/)
* class [FilterColumn](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


