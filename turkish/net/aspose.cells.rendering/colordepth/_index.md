---
title: "Enum ColorDepth"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Rendering.ColorDepth enum. TIFF görüntüsü için Bit Derinliği Türünü listeler."
type: docs
url: /tr/net/aspose.cells.rendering/colordepth/
---
## ColorDepth enumeration

Tiff görüntüsü için Bit Derinliği Türünü sıralar.

```csharp
public enum ColorDepth
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Default | `0` | Varsayılan değer, ayarlanmamış değer. |
| Format1bpp | `1` | Piksel başına 1 bit |
| Format4bpp | `4` | Piksel başına 4 bit |
| Format8bpp | `8` | Piksel başına 8 bit |
| Format24bpp | `24` | Piksel başına 24 bit |
| Format32bpp | `32` | Piksel başına 32 bit |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using Aspose.Cells.Drawing;
    using System;

    public class RenderingClassColorDepthDemo
    {
        public static void Run()
        {
            // Örnek verilerle yeni bir çalışma kitabı oluşturun
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("TIFF Color Depth Demonstration");
            worksheet.Cells["B2"].PutValue(12345);
            
            // TIFF görüntü seçeneklerini yapılandırın
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = ImageType.Tiff;
            options.TiffColorDepth = ColorDepth.Format8bpp;

            // Çalışma sayfasını belirtilen renk derinliğiyle TIFF'ye renderlayın
            SheetRender renderer = new SheetRender(worksheet, options);
            renderer.ToImage(0, "output_8bpp.tiff");

            // Başka bir renk derinliği varyantını gösterin
            options.TiffColorDepth = ColorDepth.Format24bpp;
            renderer = new SheetRender(worksheet, options);
            renderer.ToImage(0, "output_24bpp.tiff");

            Console.WriteLine("TIFF files created with different color depths.");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


