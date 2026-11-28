---
title: "Worksheet.IsGridlinesVisible"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Worksheet özelliği. Izgara çizgilerinin görünür olup olmadığını belirten bir değeri alır veya ayarlar. Varsayılan değer true'tur"
type: docs
url: /tr/net/aspose.cells/worksheet/isgridlinesvisible/
---
## Worksheet.IsGridlinesVisible property

Kılavuz çizgilerinin görünür olup olmadığını gösteren değeri alır veya ayarlar. Varsayılan değer true'tur.

```csharp
public bool IsGridlinesVisible { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyIsGridlinesVisibleDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Izgara çizgileri görünürlüğünü true olarak ayarlayın
            worksheet.IsGridlinesVisible = true;
            
            // Izgara çizgileri görmek için bazı örnek veriler ekleyin.
            worksheet.Cells["A1"].PutValue("Gridlines Visible Example");
            worksheet.Cells["A2"].PutValue("This worksheet shows gridlines");
            
            // Daha iyi görünürlük için sütunları otomatik sığdır
            worksheet.AutoFitColumns();
            
            // Çalışma kitabını kaydedin
            workbook.Save("GridlinesVisibleDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


