---
title: "FilterColumn.Top10Filter"
second_title: "Aspose.Cells için .NET API Referansı"
description: "FilterColumn özelliği. Verileri sıralamaya göre filtrelemek için Top10Filter'ı alır"
type: docs
url: /tr/net/aspose.cells/filtercolumn/top10filter/
---
## FilterColumn.Top10Filter property

Verileri sıralamaya göre filtrelemek için `Top10Filter`'ı alır.

```csharp
public Top10Filter Top10Filter { get; }
```

### Açıklamalar

Bu özelliği kullanmadan önce, lütfen [`FilterType`](../filtertype/) değerinin Top10 olduğundan emin olun, aksi takdirde null dönecektir.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FilterColumnPropertyTop10FilterDemo
    {
        public static void Run()
        {
            try
            {
                // Yeni bir çalışma kitabı oluşturun ve ilk çalışma sayfasını alın.
                Workbook workbook = new Workbook();
                Worksheet sheet = workbook.Worksheets[0];

                // Biraz örnek veri doldurun
                sheet.Cells["A1"].PutValue("Values");
                sheet.Cells["A2"].PutValue(10);
                sheet.Cells["A3"].PutValue(20);
                sheet.Cells["A4"].PutValue(30);
                sheet.Cells["A5"].PutValue(40);

                // Veri aralığına bir AutoFilter uygulayın
                sheet.AutoFilter.Range = "A1:A5";

                // İlk filtre sütununu alın (sütun indeksi 0)
                FilterColumn filterColumn = sheet.AutoFilter.FilterColumns[0];

                // Mevcut Filter nesnesini göster (null olabilir)
                Console.WriteLine("Current Filter object type: " +
                    (filterColumn.Filter != null ? filterColumn.Filter.GetType().FullName : "null"));

                // Uygulanan filtrenin Top10Filter olup olmadığını kontrol edin
                if (filterColumn.Filter != null && filterColumn.Filter.GetType().Name == "Top10Filter")
                {
                    Console.WriteLine("The filter column contains a Top10Filter.");
                }
                else
                {
                    Console.WriteLine("No Top10Filter is applied to this column.");
                }

                // Çalışma kitabını kaydedin (isteğe bağlı)
                workbook.Save("Top10FilterDemo.xlsx");
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

* class [Top10Filter](../../top10filter/)
* class [FilterColumn](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


