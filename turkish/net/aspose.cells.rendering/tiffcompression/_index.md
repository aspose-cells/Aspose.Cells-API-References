---
title: "Enum TiffCompression"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Rendering.TiffCompression enum. Görüntüleri TIFF format dosyasına kaydederken uygulanacak sıkıştırma türünü belirtir"
type: docs
url: /tr/net/aspose.cells.rendering/tiffcompression/
---
## TiffCompression enumeration

Görüntüleri TIFF format dosyasına kaydederken uygulanacak sıkıştırma türünü belirtir.

```csharp
public enum TiffCompression
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| CompressionNone | `0` | Sıkıştırma uygulanmadığını belirtir. |
| CompressionRle | `1` | RLE sıkıştırma şemasını belirtir. |
| CompressionLZW | `2` | LZW sıkıştırma şemasını belirtir. |
| CompressionCCITT3 | `3` | CCITT3 sıkıştırma şemasını belirtir. |
| CompressionCCITT4 | `4` | CCITT4 sıkıştırma şemasını belirtir. |

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class RenderingClassTiffCompressionDemo
    {
        public static void Run()
        {
            // Örnek verilerle yeni bir çalışma kitabı oluşturun
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];
            ws.Cells["A1"].PutValue("TIFF Compression Test");
            ws.Cells["A2"].PutValue(DateTime.Now.ToString());

            // Görüntü seçeneklerini ayarla
            ImageOrPrintOptions imgOpt = new ImageOrPrintOptions();
            imgOpt.HorizontalResolution = 300;
            imgOpt.VerticalResolution = 300;
            imgOpt.ImageType = ImageType.Tiff;

            // Farklı sıkıştırma türlerini test et
            string outputPath = "output_compression_";

            // LZW Sıkıştırma
            imgOpt.TiffCompression = TiffCompression.CompressionLZW;
            new WorkbookRender(wb, imgOpt).ToImage(outputPath + "LZW.tiff");

            // CCITT3 Sıkıştırma
            imgOpt.TiffCompression = TiffCompression.CompressionCCITT3;
            new WorkbookRender(wb, imgOpt).ToImage(outputPath + "CCITT3.tiff");

            // CCITT4 Sıkıştırma
            imgOpt.TiffCompression = TiffCompression.CompressionCCITT4;
            new WorkbookRender(wb, imgOpt).ToImage(outputPath + "CCITT4.tiff");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


