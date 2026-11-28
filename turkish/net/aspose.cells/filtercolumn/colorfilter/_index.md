---
title: "FilterColumn.ColorFilter"
second_title: "Aspose.Cells için .NET API Referansı"
description: "FilterColumn özelliği. Renk ile veri filtrelemek için ColorFilter'ı alır"
type: docs
url: /tr/net/aspose.cells/filtercolumn/colorfilter/
---
## FilterColumn.ColorFilter property

Renk ile veri filtrelemek için [`ColorFilter`](../../colorfilter/) alır.

```csharp
public ColorFilter ColorFilter { get; }
```

### Açıklamalar

İlk olarak [`FilterType`](../filtertype/) değerini ColorFilter olarak ayarlar, aksi takdirde Null döndürülür.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FilterColumnPropertyColorFilterDemo
    {
        public static void Run()
        {
            try
            {
                // Yeni bir çalışma kitabı oluştur
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Renkli örnek veri ekle
                worksheet.Cells["A1"].PutValue("Color");
                worksheet.Cells["A2"].PutValue("Red");
                worksheet.Cells["A3"].PutValue("Blue");
                worksheet.Cells["A4"].PutValue("Green");

                // Otomatik filtre uygula
                worksheet.AutoFilter.Range = "A1:A4";

                // Filtre sütununu alın
                FilterColumn filterColumn = worksheet.AutoFilter.FilterColumns[0];

                // ColorFilter özelliğine eriş (yalnızca okunur)
                ColorFilter colorFilter = filterColumn.ColorFilter;

                // ColorFilter özelliklerini göster
                if (colorFilter != null)
                {
                    Console.WriteLine("ColorFilter is not null");
                    Console.WriteLine("FilterByFillColor: " + colorFilter.FilterByFillColor);
                }
                else
                {
                    Console.WriteLine("ColorFilter is null (no color filter applied)");
                }

                // Çalışma kitabını kaydedin
                workbook.Save("ColorFilterDemo.xlsx");
                Console.WriteLine("ColorFilter demonstration completed successfully.");
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

* class [ColorFilter](../../colorfilter/)
* class [FilterColumn](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


