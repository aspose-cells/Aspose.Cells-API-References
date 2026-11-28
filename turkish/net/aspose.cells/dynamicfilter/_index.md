---
title: "Class DynamicFilter"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.DynamicFilter class. Dinamik filtreyi temsil eder."
type: docs
url: /tr/net/aspose.cells/dynamicfilter/
---
## DynamicFilter class

Dinamik filtreyi temsil eder.

```csharp
public class DynamicFilter
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [DynamicFilterType](../../aspose.cells/dynamicfilter/dynamicfiltertype/) { get; set; } | Bu dinamik filtrenin türünü alır ve ayarlar. |
| [MaxValue](../../aspose.cells/dynamicfilter/maxvalue/) { get; set; } | Dinamik filtrenin maksimum değerini alır ve ayarlar. |
| [Value](../../aspose.cells/dynamicfilter/value/) { get; set; } | Dinamik filtrenin değerini alır ve ayarlar. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsClassDynamicFilterDemo
    {
        public static void Run()
        {
            try
            {
                // Bir çalışma kitabı ve bir çalışma sayfası oluşturun (bağlam için isteğe bağlı)
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];
                worksheet.Name = "DemoSheet";

                // Bazı örnek sayısal verileri doldurun
                worksheet.Cells["A1"].PutValue("Numbers");
                worksheet.Cells["A2"].PutValue(10);
                worksheet.Cells["A3"].PutValue(20);
                worksheet.Cells["A4"].PutValue(30);
                worksheet.Cells["A5"].PutValue(40);
                worksheet.Cells["A6"].PutValue(50);

                // Bir otomatik filtre aralığı tanımlayın
                worksheet.AutoFilter.Range = "A1:A6";

                // İlk sütuna (AboveAverage) dinamik filtre uygula
                worksheet.AutoFilter.DynamicFilter(0, DynamicFilterType.AboveAverage);

                // AutoFilter tarafından oluşturulan DynamicFilter örneğini alın
                DynamicFilter filter = (DynamicFilter)worksheet.AutoFilter.FilterColumns[0].Filter;

                // İstenirse ek özellikler ayarlayın
                filter.Value = 25;      // Example custom value
                filter.MaxValue = 45;   // Example max value

                // Ayarlanan özellikleri göster
                Console.WriteLine($"DynamicFilterType: {filter.DynamicFilterType}");
                Console.WriteLine($"Value: {filter.Value}");
                Console.WriteLine($"MaxValue: {filter.MaxValue}");

                // Değişiklikleri uygulamak için filtreyi yenileyin
                worksheet.AutoFilter.Refresh();

                // Çalışma kitabını kaydedin (filtrelenmiş veri kaydedilecektir)
                workbook.Save("DynamicFilterDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with DynamicFilter: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


