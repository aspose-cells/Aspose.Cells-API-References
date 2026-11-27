---
title: "Klass AdvancedFilter"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.AdvancedFilter-klass. Representerar inställningarna för det avancerade filtret"
type: docs
url: /sv/net/aspose.cells/advancedfilter/
---
## AdvancedFilter class

Representerar inställningarna för det avancerade filtret.

```csharp
public class AdvancedFilter
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [CopyToRange](../../aspose.cells/advancedfilter/copytorange/) { get; } | Hämtar området där resultatet av detta avancerade filter kopieras till. |
| [CriteriaRange](../../aspose.cells/advancedfilter/criteriarange/) { get; } | Hämtar kriterieområdet för detta avancerade filter. |
| [ListRange](../../aspose.cells/advancedfilter/listrange/) { get; } | Hämtar listområdet för detta avancerade filter. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsClassAdvancedFilterDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok och hämta det första kalkylbladet
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Fyll i exempeldata för listområdet
                worksheet.Cells["A1"].PutValue("Product");
                worksheet.Cells["B1"].PutValue("Price");
                worksheet.Cells["A2"].PutValue("Apple");
                worksheet.Cells["B2"].PutValue(1.5);
                worksheet.Cells["A3"].PutValue("Banana");
                worksheet.Cells["B3"].PutValue(0.8);
                worksheet.Cells["A4"].PutValue("Orange");
                worksheet.Cells["B4"].PutValue(1.2);

                // Fyll i kriterieområdet
                worksheet.Cells["D1"].PutValue("Product");
                worksheet.Cells["D2"].PutValue("Apple");

                // Hämta AdvancedFilter-instansen från kalkylbladet
                AdvancedFilter advancedFilter = worksheet.GetAdvancedFilter();

                // Visa skrivskyddade egenskaper
                Console.WriteLine("List Range: " + advancedFilter.ListRange);
                Console.WriteLine("Criteria Range: " + advancedFilter.CriteriaRange);
                Console.WriteLine("Copy To Range: " + advancedFilter.CopyToRange);

                // Spara arbetsboken
                workbook.Save("AdvancedFilterDemo.xlsx");
                Console.WriteLine("AdvancedFilter demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in AdvancedFilter demonstration: {ex.Message}");
            }
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


