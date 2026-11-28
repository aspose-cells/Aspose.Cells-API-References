---
title: "CustomFilter.Criteria"
second_title: "Aspose.Cells için .NET API Referansı"
description: "CustomFilter özelliği. Kriterleri alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells/customfilter/criteria/
---
## CustomFilter.Criteria property

Kriteri alır ve ayarlar.

```csharp
public object Criteria { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CustomFilterPropertyCriteriaDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri ekleyin.
            worksheet.Cells["A1"].PutValue("Numbers");
            worksheet.Cells["A2"].PutValue(2);
            worksheet.Cells["A3"].PutValue(7);
            worksheet.Cells["A4"].PutValue(5);
            worksheet.Cells["A5"].PutValue(9);
            worksheet.Cells["A6"].PutValue(3);

            // Otomatik filtre uygula
            worksheet.AutoFilter.Range = "A1:A6";
            AutoFilter autoFilter = worksheet.AutoFilter;
            
            // Özel filtre ekle
            int fieldIndex = 0;
            autoFilter.Custom(fieldIndex, FilterOperatorType.GreaterOrEqual, 5);
            
            // Filtre sütununu al ve kriterleri göster
            FilterColumn fc = autoFilter.FilterColumns[fieldIndex];
            CustomFilter cf = ((CustomFilterCollection)fc.Filter)[0];
            Console.WriteLine("Filter Criteria: " + cf.Criteria);
            
            // Filtreyi yenile
            autoFilter.Refresh();
            
            // Çalışma kitabını kaydedin
            workbook.Save("CustomFilterExample.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [CustomFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


