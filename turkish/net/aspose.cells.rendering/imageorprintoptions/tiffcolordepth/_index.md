---
title: "ImageOrPrintOptions.TiffColorDepth"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ImageOrPrintOptions özelliği. Sayfaları Tiff formatında kaydederken uygulanacak bit derinliğini alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells.rendering/imageorprintoptions/tiffcolordepth/
---
## ImageOrPrintOptions.TiffColorDepth property

`Tiff` formatına sayfalar kaydedilirken yalnızca uygulanacak bit derinliğini alır veya ayarlar.

```csharp
public ColorDepth TiffColorDepth { get; set; }
```

### Açıklamalar

Yalnızca TIFF olarak kaydederken etkili olur. TiffCompression CCITT3 veya CCITT4 olarak ayarlanmışsa bu etkili olmaz, oluşturulan tiff görüntüsünün bit derinliği her zaman 1 olur.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Rendering;
    using System;

    public class ImageOrPrintOptionsPropertyTiffColorDepthDemo
    {
        public static void Run()
        {
            // Örnek veri içeren bir çalışma kitabı oluşturun.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Renk derinliğini göstermek için biçimlendirilmiş içerik ekleyin
            worksheet.Cells["A1"].PutValue("TIFF Color Depth Demonstration");
            Cell cell = worksheet.Cells["B3"];
            cell.PutValue("24-bit Color Depth");
            Style style = cell.GetStyle();
            style.Font.Color = System.Drawing.Color.FromArgb(255, 0, 128, 0);
            style.BackgroundColor = System.Drawing.Color.FromArgb(255, 255, 192, 128);
            style.Pattern = BackgroundType.Solid;
            cell.SetStyle(style);

            // TIFF renderleme için ImageOrPrintOptions başlatın
            ImageOrPrintOptions options = new ImageOrPrintOptions
            {
                ImageType = ImageType.Tiff,
                TiffCompression = TiffCompression.CompressionLZW
            };

            // TiffColorDepth değerini göster ve değiştir
            Console.WriteLine($"Initial TiffColorDepth: {options.TiffColorDepth}");
            
            // Varsayılan derinlikle renderla (1bpp)
            SheetRender renderer = new SheetRender(worksheet, options);
            renderer.ToTiff("DefaultDepthOutput.tiff");

            // 24-bit renk derinliğine değiştir
            options.TiffColorDepth = ColorDepth.Format24bpp;
            Console.WriteLine($"Modified TiffColorDepth: {options.TiffColorDepth}");

            // Yeni derinlikle renderla
            renderer.ToTiff("24BitDepthOutput.tiff");

            Console.WriteLine("Generated TIFF files with different color depths.");
        }
    }
}
```

### Ayrıca Bakınız

* enum [ColorDepth](../../colordepth/)
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


