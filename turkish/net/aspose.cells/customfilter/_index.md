---
title: "Sınıf CustomFilter"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.CustomFilter sınıf. Özel filtreyi temsil eder"
type: docs
url: /tr/net/aspose.cells/customfilter/
---
## CustomFilter class

Özel filtreyi temsil eder.

```csharp
public class CustomFilter
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Criteria](../../aspose.cells/customfilter/criteria/) { get; set; } | Kriteri alır ve ayarlar. |
| [FilterOperatorType](../../aspose.cells/customfilter/filteroperatortype/) { get; set; } | Filtre operatör tipini alır ve ayarlar. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [SetCriteria](../../aspose.cells/customfilter/setcriteria/)(FilterOperatorType, object) | Filtre kriterini ayarlar. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsClassCustomFilterDemo
    {
        public static void Run()
        {
            // Demonstrasyon için yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Çalışma sayfasına örnek veri ekle
                worksheet.Cells["A1"].PutValue("Values");
                worksheet.Cells["A2"].PutValue(10);
                worksheet.Cells["A3"].PutValue(20);
                worksheet.Cells["A4"].PutValue(30);
                worksheet.Cells["A5"].PutValue(40);

                // Aralığa otomatik filtre uygula
                worksheet.AutoFilter.Range = "A1:A5";
                AutoFilter filter = worksheet.AutoFilter;

                // Bir özel filtre uygulayarak CustomFilter örneği elde edin
                filter.Custom(0, FilterOperatorType.GreaterThan, 25);

                // Filtre koleksiyonundan ilk özel filtreyi alın
                CustomFilter customFilter = ((CustomFilterCollection)filter.FilterColumns[0].Filter)[0];

                // Filtre özelliklerini göster
                Console.WriteLine("Filter Operator: " + customFilter.FilterOperatorType);
                Console.WriteLine("Criteria Value: " + customFilter.Criteria);

                // SetCriteria metodunu kullanarak filtre kriterini değiştirin
                customFilter.SetCriteria(FilterOperatorType.LessThan, 35);

                // Güncellenmiş filtre özelliklerini göster
                Console.WriteLine("Updated Filter Operator: " + customFilter.FilterOperatorType);
                Console.WriteLine("Updated Criteria Value: " + customFilter.Criteria);

                // Çalışma kitabını kaydedin
                workbook.Save("CustomFilterDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with CustomFilter: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


