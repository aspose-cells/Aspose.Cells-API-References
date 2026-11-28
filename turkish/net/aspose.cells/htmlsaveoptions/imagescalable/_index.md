---
title: "HtmlSaveOptions.ImageScalable"
second_title: "Aspose.Cells için .NET API Referansı"
description: "HtmlSaveOptions özelliği. Sütun genişliğini tanımlamak için ölçeklenebilir birim kullanılırken, resim genişliğini tanımlamak için ölçeklenebilir birim kullanılıp kullanılmayacağını gösterir. Varsayılan değer true'tur"
type: docs
url: /tr/net/aspose.cells/htmlsaveoptions/imagescalable/
---
## HtmlSaveOptions.ImageScalable property

Sütun genişliğini tanımlamak için ölçeklenebilir birim kullanırken görüntü genişliğini ölçeklenebilir birimle tanımlayıp tanımlamayacağını gösterir. Varsayılan değer true'tur.

```csharp
public bool ImageScalable { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyImageScalableDemo
    {
        public static void Run()
        {
            // Bir örnek çalışma kitabı oluştur ve bir görüntü ekle
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Çalışma sayfasına bir örnek görüntü ekle
            int imgIndex = worksheet.Pictures.Add(0, 0, "example.jpg");
            Aspose.Cells.Drawing.Picture picture = worksheet.Pictures[imgIndex];

            // ImageScalable özelliği ile HTML kaydetme seçeneklerini ayarlayın
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.ImageScalable = false; // Images won't scale with the HTML content
            
            // Çalışma kitabını HTML olarak kaydet
            workbook.Save("output.html", saveOptions);
            
            Console.WriteLine("HTML file saved with ImageScalable set to false.");
        }
    }
}
```

### Ayrıca Bakınız

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


