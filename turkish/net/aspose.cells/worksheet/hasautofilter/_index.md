---
title: "Worksheet.HasAutofilter"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Worksheet özelliği. Bu çalışma sayfasının otomatik filtreye sahip olup olmadığını gösterir"
type: docs
url: /tr/net/aspose.cells/worksheet/hasautofilter/
---
## Worksheet.HasAutofilter property

Bu çalışma sayfasının otomatik filtreye sahip olup olmadığını gösterir.

```csharp
public bool HasAutofilter { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyHasAutofilterDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Örnek veri ekleyin.
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);
            
            // Otomatik filtreyi ayarla
            worksheet.AutoFilter.Range = "A1:B3";
            
            // Çalışma sayfasının otomatik filtreye sahip olup olmadığını kontrol et
            Console.WriteLine("Worksheet has autofilter: " + worksheet.HasAutofilter);
            
            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


