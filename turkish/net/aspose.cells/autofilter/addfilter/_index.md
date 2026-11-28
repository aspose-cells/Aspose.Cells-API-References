---
title: "AutoFilter.AddFilter"
second_title: "Aspose.Cells için .NET API Referansı"
description: "AutoFilter yöntemi. Bir filtre sütunu için bir filtre ekler"
type: docs
url: /tr/net/aspose.cells/autofilter/addfilter/
---
## AutoFilter.AddFilter method

Bir filtre sütunu için filtre ekler.

```csharp
public void AddFilter(int fieldIndex, string criteria)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fieldIndex | Int32 | Filtreyi temellendirmek istediğiniz alanın tam sayı ofseti (listenin solundan; en soldaki alan field 0'dır). |
| kriter | String | Belirtilen ölçüt (bir dize; örneğin, "101"). Sadece null olabilir veya bu sütundaki hücrelerin değerlerinden biri olabilir. |

### Açıklamalar

MS Excel 2007, bir filtre sütununda çoklu seçim destekler.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFilterMethodAddFilterWithInt32StringDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Örnek veri ekleyin.
            worksheet.Cells["A1"].PutValue("Fruits");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["A4"].PutValue("Cherry");
            worksheet.Cells["A5"].PutValue("Date");
            worksheet.Cells["A6"].PutValue("Elderberry");
            
            // Otomatik filtre aralığını oluştur
            worksheet.AutoFilter.Range = "A1:A6";
            
            // Otomatik filtreyi al
            AutoFilter filter = worksheet.AutoFilter;
            
            // 'A' ve 'E' ile başlayan değerler için filtreler ekle
            filter.AddFilter(0, "A*");
            filter.AddFilter(0, "E*");
            
            // Filtreyi yenile
            filter.Refresh();
            
            // Çalışma kitabını kaydedin
            workbook.Save("AutoFilterAddFilterDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


