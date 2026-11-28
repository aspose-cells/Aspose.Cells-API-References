---
title: "Sınıf AdvancedFilter"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.AdvancedFilter sınıfı. Gelişmiş filtrenin ayarlarını temsil eder"
type: docs
url: /tr/net/aspose.cells/advancedfilter/
---
## AdvancedFilter class

Gelişmiş filtre ayarlarını temsil eder.

```csharp
public class AdvancedFilter
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [CopyToRange](../../aspose.cells/advancedfilter/copytorange/) { get; } | Bu gelişmiş filtrenin sonucunun kopyalanacağı aralığı alır. |
| [CriteriaRange](../../aspose.cells/advancedfilter/criteriarange/) { get; } | Bu gelişmiş filtrenin kriter aralığını alır. |
| [ListRange](../../aspose.cells/advancedfilter/listrange/) { get; } | Bu gelişmiş filtrenin liste aralığını alır. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsClassAdvancedFilterDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluşturun ve ilk çalışma sayfasını alın.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Liste aralığı için örnek verileri doldurun
                worksheet.Cells["A1"].PutValue("Product");
                worksheet.Cells["B1"].PutValue("Price");
                worksheet.Cells["A2"].PutValue("Apple");
                worksheet.Cells["B2"].PutValue(1.5);
                worksheet.Cells["A3"].PutValue("Banana");
                worksheet.Cells["B3"].PutValue(0.8);
                worksheet.Cells["A4"].PutValue("Orange");
                worksheet.Cells["B4"].PutValue(1.2);

                // Kriter aralığını doldurun
                worksheet.Cells["D1"].PutValue("Product");
                worksheet.Cells["D2"].PutValue("Apple");

                // Çalışma sayfasından AdvancedFilter örneğini alın
                AdvancedFilter advancedFilter = worksheet.GetAdvancedFilter();

                // Yalnızca okunabilir özellikleri gösterin
                Console.WriteLine("List Range: " + advancedFilter.ListRange);
                Console.WriteLine("Criteria Range: " + advancedFilter.CriteriaRange);
                Console.WriteLine("Copy To Range: " + advancedFilter.CopyToRange);

                // Çalışma kitabını kaydedin
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

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


