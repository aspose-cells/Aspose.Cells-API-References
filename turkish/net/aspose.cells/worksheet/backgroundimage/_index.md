---
title: "Worksheet.BackgroundImage"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Worksheet özelliği. Çalışma sayfası arka plan görüntüsünü alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells/worksheet/backgroundimage/
---
## Worksheet.BackgroundImage property

Çalışma sayfası arka plan görüntüsünü alır ve ayarlar.

```csharp
public byte[] BackgroundImage { get; set; }
```

### Örnekler

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyBackgroundImageDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasını al
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Görüntü dosyasının yolu
            string imagePath = "background.jpg";
            
            // Görüntü dosyasını bayt dizisine oku
            byte[] imageData = File.ReadAllBytes(imagePath);
            
            // Çalışma sayfası için arka plan görüntüsünü ayarla
            worksheet.BackgroundImage = imageData;
            
            // Çalışma kitabını kaydedin
            workbook.Save("WorksheetWithBackground.xlsx");
            
            Console.WriteLine("Worksheet background image set successfully.");
        }
    }
}
```

### Ayrıca Bakınız

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


