---
title: "DynamicFilter.MaxValue"
second_title: "Aspose.Cells için .NET API Referansı"
description: "DynamicFilter özelliği. Dinamik filtre maksimum değerini alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells/dynamicfilter/maxvalue/
---
## DynamicFilter.MaxValue property

Dinamik filtrenin maksimum değerini alır ve ayarlar.

```csharp
public object MaxValue { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DynamicFilterPropertyMaxValueDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek sayısal veri ekle
            worksheet.Cells["A1"].PutValue("Values");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(20);
            worksheet.Cells["A4"].PutValue(30);
            worksheet.Cells["A5"].PutValue(40);
            worksheet.Cells["A6"].PutValue(50);

            // Otomatik filtre oluştur
            worksheet.AutoFilter.Range = "A1:A6";
            
            // Aralık kriteriyle dinamik filtre uygula
            worksheet.AutoFilter.DynamicFilter(0, DynamicFilterType.AboveAverage);
            DynamicFilter filter = (DynamicFilter)worksheet.AutoFilter.FilterColumns[0].Filter;

            // Mevcut MaxValue değerini göster
            Console.WriteLine("Current MaxValue: " + filter.MaxValue);

            // DynamicFilterType.Between mevcut olmadığından, farklı bir yaklaşım kullanacağız
            // Örneğin, bunun yerine özel bir filtre kullanabiliriz
            worksheet.AutoFilter.Custom(0, FilterOperatorType.GreaterOrEqual, 20);
            worksheet.AutoFilter.Custom(0, FilterOperatorType.LessOrEqual, 40);

            // Filtreyi uygula
            worksheet.AutoFilter.Refresh();

            // Sonucu kaydet
            workbook.Save("DynamicFilterMaxValueDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [DynamicFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


