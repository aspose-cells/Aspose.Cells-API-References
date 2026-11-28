---
title: "OdsPageBackground.Type"
second_title: "Aspose.Cells için .NET API Referansı"
description: "OdsPageBackground özelliği. Sayfa arka plan türünü alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.ods/odspagebackground/type/
---
## OdsPageBackground.Type property

Sayfa arka plan tipini alır ve ayarlar.

```csharp
public OdsPageBackgroundType Type { get; set; }
```

### Örnekler

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Ods;

namespace AsposeCellsExamples
{
    public class OdsPageBackgroundPropertyTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasının sayfa ayarına erişin
            PageSetup ps = workbook.Worksheets[0].PageSetup;
            
            // ODS sayfa arka planını alın
            OdsPageBackground background = ps.ODSPageBackground;
            
            // Arka plan türünü grafik olarak ayarlayın ve yapılandırın
            background.Type = OdsPageBackgroundType.Graphic;
            background.GraphicData = File.ReadAllBytes("image1.png");
            background.GraphicType = OdsPageBackgroundGraphicType.Area;
            
            // Çalışma kitabını kaydedin
            workbook.Save("output.ods");
            
            // Ayarları doğrulamak için kaydedilen dosyayı yeniden yükleyin
            Workbook verifyWorkbook = new Workbook("output.ods");
            PageSetup verifyPs = verifyWorkbook.Worksheets[0].PageSetup;
            OdsPageBackground verifyBackground = verifyPs.ODSPageBackground;
            
            // Doğrulama sonuçlarını çıktı olarak verin
            Console.WriteLine("Background Type: " + verifyBackground.Type);
            Console.WriteLine("Graphic Type: " + verifyBackground.GraphicType);
        }
    }
}
```

### Ayrıca Bakınız

* enum [OdsPageBackgroundType](../../odspagebackgroundtype/)
* class [OdsPageBackground](../)
* namespace [Aspose.Cells.Ods](../../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../../)


