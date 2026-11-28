---
title: "Worksheet.Zoom"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Worksheet özelliği. Yüzde olarak ölçekleme faktörünü temsil eder. 10 ile 400 arasında olmalıdır"
type: docs
url: /tr/net/aspose.cells/worksheet/zoom/
---
## Worksheet.Zoom property

Yüzde olarak ölçekleme faktörünü temsil eder. 10 ile 400 arasında olmalıdır.

```csharp
public int Zoom { get; set; }
```

### Açıklamalar

Lütfen önce görünüm tipini ayarlayın.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyZoomDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Yakınlaştırma faktörünü %120 olarak ayarla
            worksheet.Zoom = 120;
            
            // Mevcut yakınlaştırma faktörünü göster
            Console.WriteLine("Current worksheet zoom: " + worksheet.Zoom + "%");
            
            // Çalışma kitabını kaydedin
            workbook.Save("WorksheetZoomDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


