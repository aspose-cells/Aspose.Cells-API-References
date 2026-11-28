---
title: "SvgImageOptions.ImageType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SvgImageOptions özelliği. Oluşturulan görüntülerin formatını alır veya ayarlar. varsayılan değer PNG"
type: docs
url: /tr/net/aspose.cells.rendering/svgimageoptions/imagetype/
---
## SvgImageOptions.ImageType property

Oluşturulan görüntülerin formatını alır veya ayarlar. Varsayılan değer: PNG.

```csharp
public override ImageType ImageType { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Rendering;
    using System;
    using System.IO;

    public class SvgImageOptionsPropertyImageTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri ve bir görsel ekle
            worksheet.Cells["A1"].PutValue("Embedded Image Type Demonstration");
            int pictureIndex = worksheet.Pictures.Add(0, 1, "inputImage.png");
            Picture picture = worksheet.Pictures[pictureIndex];

            // SVG renderleme seçenekleri oluştur
            SvgImageOptions svgOptions = new SvgImageOptions();

            // Geçerli ImageType'ı göster (varsayılan: PNG)
            Console.WriteLine("Current ImageType: " + svgOptions.ImageType);

            // Gömülü raster görüntüler için görüntü formatını değiştir
            svgOptions.ImageType = ImageType.Jpeg;

            // Çalışma sayfası içeriğini farklı görüntü formatlarıyla SVG olarak kaydet
            using (MemoryStream stream = new MemoryStream())
            {
                picture.ToImage(stream, svgOptions);
                File.WriteAllBytes("output_with_jpeg.svg", stream.ToArray());
            }

            // PNG formatına sıfırla
            svgOptions.ImageType = ImageType.Png;
            
            using (MemoryStream stream = new MemoryStream())
            {
                picture.ToImage(stream, svgOptions);
                File.WriteAllBytes("output_with_png.svg", stream.ToArray());
            }

            Console.WriteLine("SVG files created with different embedded image formats.");
        }
    }
}
```

### Ayrıca Bakınız

* enum [ImageType](../../../aspose.cells.drawing/imagetype/)
* class [SvgImageOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


