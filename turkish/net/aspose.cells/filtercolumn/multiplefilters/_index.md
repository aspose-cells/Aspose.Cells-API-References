---
title: "FilterColumn.MultipleFilters"
second_title: "Aspose.Cells için .NET API Referansı"
description: "FilterColumn özelliği. Etiketler veya tarih/saat ile veri filtrelemek için MultipleFilterCollection'ı alır"
type: docs
url: /tr/net/aspose.cells/filtercolumn/multiplefilters/
---
## FilterColumn.MultipleFilters property

Etiketler veya tarih/saat ile veri filtrelemek için [`MultipleFilterCollection`](../../multiplefiltercollection/) alır.

```csharp
[Obsolete("Use FilterColumn.FilterValues instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public MultipleFilterCollection MultipleFilters { get; set; }
```

### Açıklamalar

NOT: Bu üye artık kullanımdan kaldırıldı. Bunun yerine FilterColumn.FilterValues özelliğini kullanın. Bu özellik, Haziran 2026'dan itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FilterColumnPropertyMultipleFiltersDemo
    {
        public static void Run()
        {
            try
            {
                // Yeni bir çalışma kitabı oluştur
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Örnek veri ekleyin.
                worksheet.Cells["A1"].PutValue("Category");
                worksheet.Cells["A2"].PutValue("Fruit");
                worksheet.Cells["A3"].PutValue("Vegetable");
                worksheet.Cells["A4"].PutValue("Fruit");
                worksheet.Cells["A5"].PutValue("Grain");

                // Aralığa Otomatik Filtre Uygula
                worksheet.AutoFilter.Range = "A1:A5";

                // İlk filtre sütununu alın
                FilterColumn filterColumn = worksheet.AutoFilter.FilterColumns[0];

                // MultipleFilters oluştur ve ayarla
                MultipleFilterCollection multipleFilters = new MultipleFilterCollection();
                multipleFilters.Add("Fruit");
                multipleFilters.Add("Vegetable");
                multipleFilters.MatchBlank = false;

                // MultipleFilters'ı filtre sütununa ata
                filterColumn.MultipleFilters = multipleFilters;

                // MultipleFilters özelliklerini göster
                Console.WriteLine("MultipleFilters Count: " + filterColumn.MultipleFilters.Count);
                Console.WriteLine("MatchBlank: " + filterColumn.MultipleFilters.MatchBlank);

                // Çalışma kitabını kaydedin
                workbook.Save("MultipleFiltersDemo.xlsx");
                Console.WriteLine("MultipleFilters demonstration completed successfully.");
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

* class [MultipleFilterCollection](../../multiplefiltercollection/)
* class [FilterColumn](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


