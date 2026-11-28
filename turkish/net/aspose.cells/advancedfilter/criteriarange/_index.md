---
title: "AdvancedFilter.CriteriaRange"
second_title: "Aspose.Cells için .NET API Referansı"
description: "AdvancedFilter özelliği. Bu gelişmiş filtrenin kriter aralığını alır"
type: docs
url: /tr/net/aspose.cells/advancedfilter/criteriarange/
---
## AdvancedFilter.CriteriaRange property

Bu gelişmiş filtrenin kriter aralığını alır.

```csharp
public string CriteriaRange { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AdvancedFilterPropertyCriteriaRangeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluşturun ve ilk çalışma sayfasını alın.
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Liste aralığı için örnek verileri doldurun
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["B1"].PutValue("Amount");
            sheet.Cells["A2"].PutValue("Food");
            sheet.Cells["B2"].PutValue(120);
            sheet.Cells["A3"].PutValue("Transport");
            sheet.Cells["B3"].PutValue(80);
            sheet.Cells["A4"].PutValue("Food");
            sheet.Cells["B4"].PutValue(150);

            // Örnek kriterleri doldurun (filtre uygulandığında bunu kullanacak)
            sheet.Cells["D1"].PutValue("Category");
            sheet.Cells["D2"].PutValue("Food");

            try
            {
                // Çalışma sayfası için AdvancedFilter nesnesini elde edin
                AdvancedFilter filter = sheet.GetAdvancedFilter();

                // ListRange, CriteriaRange ve CopyToRange özellikleri yalnızca okunabilir.
                // Otomatik olarak belirlenen aralıkları göster.
                Console.WriteLine("List Range:    " + filter.ListRange);
                Console.WriteLine("Criteria Range:" + filter.CriteriaRange);
                Console.WriteLine("Copy To Range: " + filter.CopyToRange);

                // Çalışma kitabını kaydedin (isteğe bağlı, dosyanın oluşturulabileceğini göstermek için)
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

### Ayrıca Bakınız

* class [AdvancedFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


