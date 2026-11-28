---
title: "OoxmlSaveOptions.UpdateZoom"
second_title: "Aspose.Cells için .NET API Referansı"
description: "OoxmlSaveOptions özelliği. PageSetup.FitToPagesWide ve PageSetup.FitToPagesTall özellikleri çalışma sayfasının ölçeklendirilmesini kontrol ediyorsa, dosyayı kaydetmeden önce ölçekleme faktörünün güncellenip güncellenmeyeceğini gösterir"
type: docs
url: /tr/net/aspose.cells/ooxmlsaveoptions/updatezoom/
---
## OoxmlSaveOptions.UpdateZoom property

PageSetup.FitToPagesWide ve PageSetup.FitToPagesTall özellikleri çalışma sayfasının nasıl ölçeklendirileceğini kontrol ediyorsa, dosyayı kaydetmeden önce ölçekleme faktörünün güncellenip güncellenmeyeceğini gösterir.

```csharp
public bool UpdateZoom { get; set; }
```

### Açıklamalar

Performans için varsayılan değer false'tur.

### Örnekler

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class OoxmlSaveOptionsPropertyUpdateZoomDemo
    {
        public static void Run()
        {
            // Örnek bir çalışma kitabı oluşturun
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // İlk yakınlaştırma seviyesini ayarla
            worksheet.PageSetup.Zoom = 100;

            // UpdateZoom etkinleştirilmiş kaydetme seçeneklerini oluştur
            OoxmlSaveOptions saveOptions = new OoxmlSaveOptions(SaveFormat.Xlsx);
            saveOptions.UpdateZoom = true;

            // Bellek akışına kaydet
            using (MemoryStream stream = new MemoryStream())
            {
                workbook.Save(stream, saveOptions);
                
                // Yakınlaştırmanın güncellendiğini doğrulamak için çalışma kitabını yeniden yükle
                stream.Position = 0;
                Workbook reloadedWorkbook = new Workbook(stream);
                Console.WriteLine("Worksheet zoom level: " + reloadedWorkbook.Worksheets[0].PageSetup.Zoom);
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [OoxmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


