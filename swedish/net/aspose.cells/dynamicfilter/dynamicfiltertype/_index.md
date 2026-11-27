---
title: "DynamicFilter.DynamicFilterType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DynamicFilter property. Hämtar och anger typen av detta dynamiska filter"
type: docs
url: /sv/net/aspose.cells/dynamicfilter/dynamicfiltertype/
---
## DynamicFilter.DynamicFilterType property

Hämtar och anger typen för detta dynamiska filter.

```csharp
public DynamicFilterType DynamicFilterType { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DynamicFilterPropertyDynamicFilterTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata med datum
            worksheet.Cells["A1"].PutValue("Date");
            worksheet.Cells["A2"].PutValue(new DateTime(2023, 1, 15));
            worksheet.Cells["A3"].PutValue(new DateTime(2023, 2, 20));
            worksheet.Cells["A4"].PutValue(new DateTime(2023, 3, 10));
            worksheet.Cells["A5"].PutValue(new DateTime(2023, 4, 5));

            try
            {
                // Skapa autofilter
                worksheet.AutoFilter.Range = "A1:A5";

                // Tillämpa dynamiskt filter för marsdatum
                worksheet.AutoFilter.DynamicFilter(0, DynamicFilterType.March);

                // Hämta DynamicFilter-instansen
                DynamicFilter filter = (DynamicFilter)worksheet.AutoFilter.FilterColumns[0].Filter;

                // Visa det aktuella DynamicFilterType‑värdet
                Console.WriteLine("Current DynamicFilterType: " + filter.DynamicFilterType);

                // Ändra filtertypen för att visa aprildatum
                filter.DynamicFilterType = DynamicFilterType.April;

                // Visa det uppdaterade DynamicFilterType‑värdet
                Console.WriteLine("Updated DynamicFilterType: " + filter.DynamicFilterType);

                // Tillämpa filtret
                worksheet.AutoFilter.Refresh();

                // Spara resultatet
                workbook.Save("DynamicFilterTypeDemo.xlsx");
                Console.WriteLine("DynamicFilterType has been demonstrated successfully.");
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

* enum [DynamicFilterType](../../dynamicfiltertype/)
* class [DynamicFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


