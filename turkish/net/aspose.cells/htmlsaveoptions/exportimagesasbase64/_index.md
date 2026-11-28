---
title: "HtmlSaveOptions.ExportImagesAsBase64"
second_title: "Aspose.Cells için .NET API Referansı"
description: "HtmlSaveOptions özelliği. Görsellerin HTML, MHTML veya EPUB formatında Base64 olarak kaydedilip kaydedilmeyeceğini belirtir."
type: docs
url: /tr/net/aspose.cells/htmlsaveoptions/exportimagesasbase64/
---
## HtmlSaveOptions.ExportImagesAsBase64 property

Görüntülerin HTML, MHTML veya EPUB formatında Base64 olarak kaydedilip kaydedilmeyeceğini belirtir.

```csharp
public bool ExportImagesAsBase64 { get; set; }
```

### Açıklamalar

Bu özellik true olarak ayarlandığında, görüntü verileri doğrudan img öğelerine gömülür ve ayrı dosyalar oluşturulmaz.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportImagesAsBase64Demo
    {
        public static void Run()
        {
            // Örnek veri içeren bir çalışma kitabı oluşturun.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Çalışma sayfasına bir resim ekle
            worksheet.Pictures.Add(0, 0, "example.jpg");
            
            // HTML kaydetme seçenekleri oluştur
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            
            // ExportImagesAsBase64 özelliğini true yaparak görüntüleri base64 dizeleri olarak gömün
            saveOptions.ExportImagesAsBase64 = true;
            
            // Çalışma kitabını gömülü görüntülerle HTML olarak kaydedin
            workbook.Save("output.html", saveOptions);
            
            Console.WriteLine("HTML with embedded images saved successfully.");
        }
    }
}
```

### Ayrıca Bakınız

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


