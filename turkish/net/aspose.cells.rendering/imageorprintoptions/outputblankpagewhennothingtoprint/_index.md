---
title: "ImageOrPrintOptions.OutputBlankPageWhenNothingToPrint"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ImageOrPrintOptions özelliği. Yazdırılacak bir şey olmadığında boş bir sayfa çıktı verilip verilmeyeceğini gösterir"
type: docs
url: /tr/net/aspose.cells.rendering/imageorprintoptions/outputblankpagewhennothingtoprint/
---
## ImageOrPrintOptions.OutputBlankPageWhenNothingToPrint property

Yazdırılacak bir şey olmadığında boş bir sayfa çıktısı verilip verilmeyeceğini gösterir.

```csharp
public bool OutputBlankPageWhenNothingToPrint { get; set; }
```

### Açıklamalar

Varsayılan değeri false'tur.

### Örnekler

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsPropertyOutputBlankPageWhenNothingToPrintDemo
    {
        public static void Run()
        {
            // Yeni boş bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Boş olan ilk çalışma sayfasına erişin
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Görüntü veya yazdırma seçeneklerini ayarla
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = Aspose.Cells.Drawing.ImageType.Png;
            options.OnePagePerSheet = true;
            
            // OutputBlankPageWhenNothingToPrint özelliğini gösterin
            options.OutputBlankPageWhenNothingToPrint = true;
            
            // Sayfayı oluştur
            SheetRender renderer = new SheetRender(worksheet, options);
            
            // Özellik ayarı nedeniyle çıktı hâlâ bir boş sayfa üretecek
            Console.WriteLine("Page count with OutputBlankPageWhenNothingToPrint=true: " + renderer.PageCount);
            
            // İlk sayfayı bellek akışına kaydet
            MemoryStream stream = new MemoryStream();
            renderer.ToImage(0, stream);
            Console.WriteLine("Image data length: " + stream.ToArray().Length);
            
            // Şimdi özelliği false olarak ayarlayın
            options.OutputBlankPageWhenNothingToPrint = false;
            SheetRender renderer2 = new SheetRender(worksheet, options);
            
            // Çıktı artık sıfır sayfa içerecek
            Console.WriteLine("Page count with OutputBlankPageWhenNothingToPrint=false: " + renderer2.PageCount);
        }
    }
}
```

### Ayrıca Bakınız

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


