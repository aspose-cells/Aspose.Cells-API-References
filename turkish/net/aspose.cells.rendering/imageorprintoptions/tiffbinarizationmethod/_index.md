---
title: "ImageOrPrintOptions.TiffBinarizationMethod"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ImageOrPrintOptions özelliği. ImageType Tiff ve TiffCompression Ccitt3 veya Ccitt4 olduğunda görüntüleri 1 bpp formatına dönüştürürken kullanılan yöntemi alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells.rendering/imageorprintoptions/tiffbinarizationmethod/
---
## ImageOrPrintOptions.TiffBinarizationMethod property

[`ImageType`](../imagetype/) Tiff ve [`TiffCompression`](../tiffcompression/) Ccitt3 veya Ccitt4 olduğunda görüntüleri 1 bpp formatına dönüştürürken kullanılan yöntemi alır veya ayarlar.

```csharp
public ImageBinarizationMethod TiffBinarizationMethod { get; set; }
```

### Açıklamalar

Varsayılan değer FloydSteinbergDithering'dir.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class ImageOrPrintOptionsPropertyTiffBinarizationMethodDemo
    {
        public static void Run()
        {
            // Örnek veriyle bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Görsel gösterim için gradyan verisi ekleyin
            for (int i = 0; i < 15; i++)
            {
                Cell cell = worksheet.Cells[i, 0];
                cell.PutValue(i * 7);
                Style style = cell.GetStyle();
                style.BackgroundColor = Color.FromArgb(i * 18, i * 18, i * 18);
                cell.SetStyle(style);
            }

            // TIFF renderleme seçeneklerini yapılandırın
            ImageOrPrintOptions options = new ImageOrPrintOptions
            {
                ImageType = ImageType.Tiff,
                TiffCompression = TiffCompression.CompressionCCITT3,
                TiffColorDepth = ColorDepth.Format1bpp
            };

            // Mevcut ikilileştirme yöntemini göster
            Console.WriteLine("Initial TiffBinarizationMethod: " + options.TiffBinarizationMethod);

            // Varsayılan eşik yöntemiyle renderlayın
            new SheetRender(worksheet, options).ToImage(0, "ThresholdBinarization.tiff");

            // Floyd-Steinberg ikilileştirmeye geçin
            options.TiffBinarizationMethod = ImageBinarizationMethod.FloydSteinbergDithering;
            Console.WriteLine("\nModified TiffBinarizationMethod: " + options.TiffBinarizationMethod);

            // Yeni yöntemle renderlayın
            new SheetRender(worksheet, options).ToImage(0, "DitheringBinarization.tiff");

            Console.WriteLine("\nGenerated TIFF files demonstrate different 1bpp conversion methods.");
        }
    }
}
```

### Ayrıca Bakınız

* enum [ImageBinarizationMethod](../../imagebinarizationmethod/)
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


