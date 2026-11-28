---
title: "DynamicFilter.DynamicFilterType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "DynamicFilter özelliği. Bu dinamik filtrenin tipini alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells/dynamicfilter/dynamicfiltertype/
---
## DynamicFilter.DynamicFilterType property

Bu dinamik filtrenin türünü alır ve ayarlar.

```csharp
public DynamicFilterType DynamicFilterType { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DynamicFilterPropertyDynamicFilterTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Tarihlerle örnek veri ekle
            worksheet.Cells["A1"].PutValue("Date");
            worksheet.Cells["A2"].PutValue(new DateTime(2023, 1, 15));
            worksheet.Cells["A3"].PutValue(new DateTime(2023, 2, 20));
            worksheet.Cells["A4"].PutValue(new DateTime(2023, 3, 10));
            worksheet.Cells["A5"].PutValue(new DateTime(2023, 4, 5));

            try
            {
                // Otomatik filtre oluştur
                worksheet.AutoFilter.Range = "A1:A5";

                // Mart tarihleri için dinamik filtre uygula
                worksheet.AutoFilter.DynamicFilter(0, DynamicFilterType.March);

                // DynamicFilter örneğini al
                DynamicFilter filter = (DynamicFilter)worksheet.AutoFilter.FilterColumns[0].Filter;

                // Mevcut DynamicFilterType değerini göster
                Console.WriteLine("Current DynamicFilterType: " + filter.DynamicFilterType);

                // Nisan tarihlerini gösterecek şekilde filtre tipini değiştir
                filter.DynamicFilterType = DynamicFilterType.April;

                // Güncellenmiş DynamicFilterType değerini göster
                Console.WriteLine("Updated DynamicFilterType: " + filter.DynamicFilterType);

                // Filtreyi uygula
                worksheet.AutoFilter.Refresh();

                // Sonucu kaydet
                workbook.Save("DynamicFilterTypeDemo.xlsx");
                Console.WriteLine("DynamicFilterType has been demonstrated successfully.");
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

* enum [DynamicFilterType](../../dynamicfiltertype/)
* class [DynamicFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


