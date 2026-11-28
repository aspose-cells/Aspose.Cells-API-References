---
title: "ImageOrPrintOptions.EmbededImageNameInSvg"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ImageOrPrintOptions özelliği. SVG içinde gömülü görüntünün dosya adını belirtir. Bu, cxpsEmbedded gibi bir dizinle tam yol olmalıdır."
type: docs
url: /tr/net/aspose.cells.rendering/imageorprintoptions/embededimagenameinsvg/
---
## ImageOrPrintOptions.EmbededImageNameInSvg property

Svg içinde gömülü görüntünün dosya adını belirtin. Bu, "c:\\xpsEmbedded" gibi bir dizinle tam yol olmalıdır.

```csharp
[Obsolete("Images are now always embedded in Svg with base64 format, please remove this property.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public string EmbededImageNameInSvg { get; set; }
```

### Açıklamalar

NOT: Bu üye artık kullanımdan kaldırıldı. Bunun yerine, görüntüler artık her zaman base64 formatında SVG'ye gömüldüğü için lütfen bu özelliği kaldırın. Bu özellik, Nisan 2025'ten itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Rendering;
    using System;
    using System.IO;

    public class ImageOrPrintOptionsPropertyEmbededImageNameInSvgDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluşturun ve ilk çalışma sayfasına erişin
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Basit bir bellek içi görüntü oluşturup çalışma sayfasına ekleyin
            byte[] redPngBytes = Convert.FromBase64String("iVBORw0KGgoAAAANSUhEUgAAAAEAAAABCAYAAAAfFcSJAAAADUlEQVR42mNkYPhfDwAChwGA60e6kgAAAABJRU5ErkJggg==");
            worksheet.Pictures.Add(0, 0, new MemoryStream(redPngBytes));

            // SVG formatında görüntü renderleme seçenekleri oluşturun
            ImageOrPrintOptions options = new ImageOrPrintOptions
            {
                ImageType = ImageType.Svg
            };

            // Mevcut gömülü görüntü yolunu göster
            Console.WriteLine("Initial EmbededImageNameInSvg: " + options.EmbededImageNameInSvg);

            // Yeni gömülü görüntü dizinini yapılandır
            string imageDir = "svg_embedded_images/";
            options.EmbededImageNameInSvg = imageDir;
            Directory.CreateDirectory(imageDir);

            // Çalışma sayfasını yapılandırılmış seçeneklerle SVG'ye renderlayın
            SheetRender renderer = new SheetRender(worksheet, options);
            renderer.ToImage(0, "worksheet_output.svg");

            Console.WriteLine("Generated SVG with embedded images in: " + Path.GetFullPath(imageDir));
        }
    }
}
```

### Ayrıca Bakınız

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


