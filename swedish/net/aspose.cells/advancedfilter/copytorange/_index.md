---
title: "AdvancedFilter.CopyToRange"
second_title: "Aspose.Cells för .NET API‑referens"
description: "AdvancedFilter‑egenskap. Hämtar intervallet där resultatet av detta avancerade filter kopieras till"
type: docs
url: /sv/net/aspose.cells/advancedfilter/copytorange/
---
## AdvancedFilter.CopyToRange property

Hämtar området där resultatet av detta avancerade filter kopieras till.

```csharp
public string CopyToRange { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AdvancedFilterPropertyCopyToRangeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Hämta det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata i kalkylbladet
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(1.5);
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["B3"].PutValue(0.8);
            worksheet.Cells["A4"].PutValue("Orange");
            worksheet.Cells["B4"].PutValue(1.2);

            // Lägg till kriterieintervall
            worksheet.Cells["D1"].PutValue("Product");
            worksheet.Cells["D2"].PutValue("Apple");

            try
            {
                // Hämta AdvancedFilter-instansen från kalkylbladet
                AdvancedFilter advancedFilter = worksheet.GetAdvancedFilter();

                // Visa värdet för CopyToRange‑egenskapen
                Console.WriteLine("CopyToRange value: " + advancedFilter.CopyToRange);

                // Spara arbetsboken
                workbook.Save("CopyToRangeDemo.xlsx");
                Console.WriteLine("CopyToRange demonstration completed successfully.");
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


