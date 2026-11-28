---
title: "FilterColumn.CustomFilters"
second_title: "Aspose.Cells için .NET API Referansı"
description: "FilterColumn özelliği. Verileri özel ölçütlere göre filtrelemek için CustomFilterCollection alır"
type: docs
url: /tr/net/aspose.cells/filtercolumn/customfilters/
---
## FilterColumn.CustomFilters property

[`CustomFilterCollection`](../../customfiltercollection/) alır; verileri özel ölçütlere göre filtrelemek için.

```csharp
public CustomFilterCollection CustomFilters { get; set; }
```

### Açıklamalar

NOT: Bu özelliğin ayarlayıcısı artık kullanımdan kaldırıldı. Bunun yerine, [`FilterType`](../filtertype/) özelliğini CustomFilters olarak ayarlayın. Bu özellik, Haziran 2026'dan itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### Örnekler

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
                // Yeni bir çalışma kitabı oluştur
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Örnek veri ekleyin.
                worksheet.Cells["A1"].PutValue("Product");
                worksheet.Cells["A2"].PutValue("Apple");
                worksheet.Cells["A3"].PutValue("Banana");
                worksheet.Cells["A4"].PutValue("Cherry");
                worksheet.Cells["A5"].PutValue("Date");
                worksheet.Cells["A6"].PutValue("Elderberry");

                // Otomatik filtre uygula
                worksheet.AutoFilter.Range = "A1:A6";

                // Filtre sütununu alın
                FilterColumn filterColumn = worksheet.AutoFilter.FilterColumns[0];

                // AutoFilter.Custom yöntemiyle özel filtreler oluşturun ve ayarlayın
                // İlk filtre: "A" ile başlar
                worksheet.AutoFilter.Custom(0, FilterOperatorType.BeginsWith, "A", false, FilterOperatorType.None, null);

                // İkinci filtre: "y" ile biter (VE ilişkisi)
                worksheet.AutoFilter.Custom(0, FilterOperatorType.EndsWith, "y", true, FilterOperatorType.None, null);

                // Filtre sütunundan özel filtreleri alın
                CustomFilterCollection customFilters = filterColumn.CustomFilters;

                // Özel filtre bilgilerini göster
                Console.WriteLine($"Number of custom filters: {customFilters.Count}");
                Console.WriteLine($"Filter relationship (And): {customFilters.And}");

                // Not: CustomFilterCollection bireysel filtreleri doğrudan ortaya çıkarmaz
                // bir indeksleyici aracılığıyla, bu yüzden yalnızca koleksiyon özelliklerini gösterebiliriz
                Console.WriteLine("Custom filters have been applied to the column.");

                // Çalışma kitabını kaydedin
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

### Ayrıca Bakınız

* class [CustomFilterCollection](../../customfiltercollection/)
* class [FilterColumn](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


