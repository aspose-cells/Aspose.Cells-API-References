---
title: "FilterColumn.DynamicFilter"
second_title: "Aspose.Cells för .NET API‑referens"
description: "FilterColumn-egenskapen. Hämtar DynamicFilter för filtrering med dynamiska kriterier"
type: docs
url: /sv/net/aspose.cells/filtercolumn/dynamicfilter/
---
## FilterColumn.DynamicFilter property

Hämtar `DynamicFilter` för filtrering med dynamiska kriterier.

```csharp
public DynamicFilter DynamicFilter { get; }
```

### Anmärkningar

Innan du använder den här egenskapen, se till att [`FilterType`](../filtertype/) är DynamicFilter, annars returneras null.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FilterColumnPropertyDynamicFilterDemo
    {
        public static void Run()
        {
            try
            {
                // Skapa en ny arbetsbok
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Lägg till exempeldata
                worksheet.Cells["A1"].PutValue("Date");
                worksheet.Cells["A2"].PutValue(DateTime.Now.AddDays(-10));
                worksheet.Cells["A3"].PutValue(DateTime.Now.AddDays(-5));
                worksheet.Cells["A4"].PutValue(DateTime.Now);

                // Applicera autofilter
                worksheet.AutoFilter.Range = "A1:A4";

                // Hämta filterkolumnen
                FilterColumn filterColumn = worksheet.AutoFilter.FilterColumns[0];

                // Åtkomst till DynamicFilter-egenskapen (skrivskyddad)
                DynamicFilter dynamicFilter = filterColumn.DynamicFilter;

                // Visa DynamicFilter-egenskaper
                if (dynamicFilter != null)
                {
                    Console.WriteLine("DynamicFilter is not null");
                    Console.WriteLine("DynamicFilterType: " + dynamicFilter.DynamicFilterType);
                    Console.WriteLine("Value: " + dynamicFilter.Value);
                    Console.WriteLine("MaxValue: " + dynamicFilter.MaxValue);
                }
                else
                {
                    Console.WriteLine("DynamicFilter is null (no dynamic filter applied)");
                }

                // Spara arbetsboken
                workbook.Save("DynamicFilterDemo.xlsx");
                Console.WriteLine("DynamicFilter demonstration completed successfully.");
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

* class [DynamicFilter](../../dynamicfilter/)
* class [FilterColumn](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


