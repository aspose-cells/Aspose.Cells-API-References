---
title: "HtmlSaveOptions.IsExpImageToTempDir"
second_title: "Aspose.Cells için .NET API Referansı"
description: "HtmlSaveOptions özelliği. Görüntü dosyalarının geçici dizine aktarılıp aktarılmayacağını gösterir. Yalnızca html akışına kaydederken kullanılır."
type: docs
url: /tr/net/aspose.cells/htmlsaveoptions/isexpimagetotempdir/
---
## HtmlSaveOptions.IsExpImageToTempDir property

Görüntü dosyalarının geçici dizine dışa aktarılıp aktarılmayacağını gösterir. Yalnızca html akışına kaydederken.

```csharp
public bool IsExpImageToTempDir { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyIsExpImageToTempDirDemo
    {
        public static void Run()
        {
            // Bir örnek çalışma kitabı oluştur ve bir görüntü ekle
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Çalışma sayfasına bir örnek görüntü ekle
            worksheet.Pictures.Add(0, 0, "https://www.aspose.com/templates/aspose/App_Themes/V3/images/cells/header/aspose_cells-for-net.png");

            // IsExpImageToTempDir etkinleştirilmiş şekilde HTML kaydetme seçeneklerini ayarla
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.IsExpImageToTempDir = true;
            options.ExportImagesAsBase64 = false; // Ensure images are exported as separate files

            // Çalışma kitabını HTML olarak kaydet
            workbook.Save("output.html", options);
            
            Console.WriteLine("HTML saved with images exported to temp directory.");
        }
    }
}
```

### Ayrıca Bakınız

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


