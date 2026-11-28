---
title: "AdvancedFilter.CopyToRange"
second_title: "Aspose.Cells için .NET API Referansı"
description: "AdvancedFilter özelliği. Bu gelişmiş filtrenin sonucunun kopyalanacağı aralığı alır"
type: docs
url: /tr/net/aspose.cells/advancedfilter/copytorange/
---
## AdvancedFilter.CopyToRange property

Bu gelişmiş filtrenin sonucunun kopyalanacağı aralığı alır.

```csharp
public string CopyToRange { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AdvancedFilterPropertyCopyToRangeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // İlk çalışma sayfasını al
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına örnek veri ekle
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(1.5);
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["B3"].PutValue(0.8);
            worksheet.Cells["A4"].PutValue("Orange");
            worksheet.Cells["B4"].PutValue(1.2);

            // Kriter aralığını ekleyin
            worksheet.Cells["D1"].PutValue("Product");
            worksheet.Cells["D2"].PutValue("Apple");

            try
            {
                // Çalışma sayfasından AdvancedFilter örneğini alın
                AdvancedFilter advancedFilter = worksheet.GetAdvancedFilter();

                // CopyToRange özelliği değerini göster
                Console.WriteLine("CopyToRange value: " + advancedFilter.CopyToRange);

                // Çalışma kitabını kaydedin
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

### Ayrıca Bakınız

* class [AdvancedFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


