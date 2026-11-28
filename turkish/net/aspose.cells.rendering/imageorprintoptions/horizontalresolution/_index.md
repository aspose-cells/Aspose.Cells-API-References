---
title: "ImageOrPrintOptions.HorizontalResolution"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ImageOrPrintOptions özelliği. Oluşturulan görüntüler için inç başına nokta cinsinden yatay çözünürlüğü alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells.rendering/imageorprintoptions/horizontalresolution/
---
## ImageOrPrintOptions.HorizontalResolution property

Oluşturulan görüntüler için yatay çözünürlüğü alır veya ayarlar, inç başına nokta (dpi) cinsinden.

```csharp
public int HorizontalResolution { get; set; }
```

### Açıklamalar

Varsayılan değer 96'dır.

`HorizontalResolution` ve [`VerticalResolution`](../verticalresolution/) ayarları, çıktı görüntüsünün piksel cinsinden genişlik ve yüksekliğini etkiler.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsPropertyHorizontalResolutionDemo
    {
        public static void Run()
        {
            // Örnek verilerle yeni bir çalışma kitabı oluşturun
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample Text for Image Rendering");

            // ImageOrPrintOptions'ı başlat
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = ImageType.Png;
            
            // Yatay ve dikey çözünürlüğü ayarla
            options.HorizontalResolution = 192;
            options.VerticalResolution = 192;

            // Belirtilen çözünürlükte çalışma sayfasını görüntüye render et
            SheetRender renderer = new SheetRender(worksheet, options);
            renderer.ToImage(0, "WorksheetImage_192dpi.png");

            // Farklı çözünürlükleri göster
            options.HorizontalResolution = 300;
            options.VerticalResolution = 300;
            renderer = new SheetRender(worksheet, options);
            renderer.ToImage(0, "WorksheetImage_300dpi.png");
        }
    }
}
```

### Ayrıca Bakınız

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


