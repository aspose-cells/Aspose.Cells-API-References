---
title: "Worksheet.IsPageBreakPreview"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Worksheet özelliği. Belirtilen çalışma sayfasının normal görünümde mi yoksa sayfa kırılımı önizlemesinde mi gösterildiğini belirtir"
type: docs
url: /tr/net/aspose.cells/worksheet/ispagebreakpreview/
---
## Worksheet.IsPageBreakPreview property

Belirtilen çalışma sayfasının normal görünümde mi yoksa sayfa kesme önizlemesinde mi gösterildiğini gösterir.

```csharp
public bool IsPageBreakPreview { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyIsPageBreakPreviewDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Çalışma sayfasını Sayfa Kırılımı Önizleme moduna ayarlayın
            worksheet.IsPageBreakPreview = true;
            
            // Demonstrasyon için yakınlaştırmayı %100'e ayarlayın
            worksheet.Zoom = 100;
            
            // Mevcut ayarları çıktı olarak verin
            Console.WriteLine("IsPageBreakPreview: " + worksheet.IsPageBreakPreview);
            Console.WriteLine("Zoom: " + worksheet.Zoom);
            
            // Çalışma kitabını kaydedin
            workbook.Save("WorksheetPropertyIsPageBreakPreviewDemo_output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


