---
title: "FilterColumn.DynamicFilter"
second_title: "Aspose.Cells için .NET API Referansı"
description: "FilterColumn özelliği. Dinamik kriterlerle filtreleme için DynamicFilter'ı alır"
type: docs
url: /tr/net/aspose.cells/filtercolumn/dynamicfilter/
---
## FilterColumn.DynamicFilter property

Dinamik kriterlerle filtreleme için `DynamicFilter` alır.

```csharp
public DynamicFilter DynamicFilter { get; }
```

### Açıklamalar

Bu özelliği kullanmadan önce lütfen [`FilterType`](../filtertype/) değerinin DynamicFilter olduğundan emin olun, aksi takdirde null döndürülür.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FilterColumnPropertyDynamicFilterDemo
    {
        public static void Run()
        {
            try
            {
                // Yeni bir çalışma kitabı oluştur
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Örnek veri ekleyin.
                worksheet.Cells["A1"].PutValue("Date");
                worksheet.Cells["A2"].PutValue(DateTime.Now.AddDays(-10));
                worksheet.Cells["A3"].PutValue(DateTime.Now.AddDays(-5));
                worksheet.Cells["A4"].PutValue(DateTime.Now);

                // Otomatik filtre uygula
                worksheet.AutoFilter.Range = "A1:A4";

                // Filtre sütununu alın
                FilterColumn filterColumn = worksheet.AutoFilter.FilterColumns[0];

                // DynamicFilter özelliğine eriş (yalnızca okuma)
                DynamicFilter dynamicFilter = filterColumn.DynamicFilter;

                // DynamicFilter özelliklerini göster
                if (dynamicFilter != null)
                {
                    Console.WriteLine("DynamicFilter is not null");
                    Console.WriteLine("DynamicFilterType: " + dynamicFilter.DynamicFilterType);
                    Console.WriteLine("Value: " + dynamicFilter.Value);
                    Console.WriteLine("MaxValue: " + dynamicFilter.MaxValue);
                }
                else
                {
                    Console.WriteLine("DynamicFilter is null (no dynamic filter applied)");
                }

                // Çalışma kitabını kaydedin
                workbook.Save("DynamicFilterDemo.xlsx");
                Console.WriteLine("DynamicFilter demonstration completed successfully.");
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

* class [DynamicFilter](../../dynamicfilter/)
* class [FilterColumn](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


