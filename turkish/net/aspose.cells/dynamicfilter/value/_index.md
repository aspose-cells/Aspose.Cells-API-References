---
title: "DynamicFilter.Value"
second_title: "Aspose.Cells için .NET API Referansı"
description: "DynamicFilter özelliği. Dinamik filtre değerini alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells/dynamicfilter/value/
---
## DynamicFilter.Value property

Dinamik filtrenin değerini alır ve ayarlar.

```csharp
public object Value { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DynamicFilterPropertyValueDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri ekleyin.
            worksheet.Cells["A1"].PutValue("Date");
            worksheet.Cells["A2"].PutValue(new DateTime(2023, 1, 15));
            worksheet.Cells["A3"].PutValue(new DateTime(2023, 2, 20));
            worksheet.Cells["A4"].PutValue(new DateTime(2023, 3, 10));
            worksheet.Cells["A5"].PutValue(new DateTime(2023, 4, 5));

            // Otomatik filtre oluştur
            worksheet.AutoFilter.Range = "A1:A5";
            worksheet.AutoFilter.DynamicFilter(0, DynamicFilterType.March);
            DynamicFilter filter = (DynamicFilter)worksheet.AutoFilter.FilterColumns[0].Filter;

            // Mevcut filtre değerini gösterin
            Console.WriteLine("Current DynamicFilter Value: " + filter.Value);

            // Nisan tarihlerini göstermek için filtre değerini değiştirin
            filter.Value = new DateTime(2023, 4, 1);
            filter.DynamicFilterType = DynamicFilterType.April;

            // Filtreyi uygula
            worksheet.AutoFilter.Refresh();

            // Sonucu kaydet
            workbook.Save("DynamicFilterValueDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [DynamicFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


