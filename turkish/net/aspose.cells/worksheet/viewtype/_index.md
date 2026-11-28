---
title: "Worksheet.ViewType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Worksheet özelliği. Görünüm türünü alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells/worksheet/viewtype/
---
## Worksheet.ViewType property

Görünüm tipini alır ve ayarlar.

```csharp
public ViewType ViewType { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyViewTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Görünüm türünü PageLayoutView olarak ayarlayın ve cetveli etkinleştirin
            worksheet.ViewType = ViewType.PageLayoutView;
            worksheet.IsRulerVisible = true;
            
            // Görünümü göstermek için örnek içerik ekleyin
            worksheet.Cells["A1"].PutValue("Page Layout View Demo");
            worksheet.Cells["A2"].PutValue("Ruler is visible in this view");
            
            // Çalışma kitabını kaydedin
            workbook.Save("WorksheetViewTypeDemo.xlsx");
            
            Console.WriteLine("Worksheet ViewType demo completed successfully.");
        }
    }
}
```

### Ayrıca Bakınız

* enum [ViewType](../../viewtype/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


