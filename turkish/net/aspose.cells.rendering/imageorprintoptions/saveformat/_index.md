---
title: "ImageOrPrintOptions.SaveFormat"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ImageOrPrintOptions özelliği. Çıktı dosya formatı tipini alır veya ayarlar. Tiff/XPS desteklenir."
type: docs
url: /tr/net/aspose.cells.rendering/imageorprintoptions/saveformat/
---
## ImageOrPrintOptions.SaveFormat property

Çıktı dosya formatı tipini alır veya ayarlar. Tiff/XPS desteklenir.

```csharp
[Obsolete("For Tiff/Svg, use ImageType; For Xps, use Workbook.Save(string, SaveOptions) with XpsSaveOptions")]
[EditorBrowsable(EditorBrowsableState.Never)]
public SaveFormat SaveFormat { get; set; }
```

### Açıklamalar

NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine, Tiff/Svg için [`ImageType`](../imagetype/); Xps için ise [`Save`](../../../aspose.cells/workbook/save/) ile [`XpsSaveOptions`](../../../aspose.cells/xpssaveoptions/) kullanın. Bu özellik, Ağustos 2022'den itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;
    using System.IO;

    public class ImageOrPrintOptionsPropertySaveFormatDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluşturun ve örnek verileri doldurun
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Aspose.Cells SaveFormat Demonstration");
            
            // ImageOrPrintOptions örneği oluşturun
            ImageOrPrintOptions options = new ImageOrPrintOptions();

            // İlk SaveFormat değerini göster
            Console.WriteLine("Initial SaveFormat: " + options.SaveFormat);

            // SaveFormat'ı TIFF olarak ayarlayın ve çalışma sayfasını işleyin
            options.SaveFormat = SaveFormat.Tiff;
            SheetRender tiffRenderer = new SheetRender(worksheet, options);
            using (FileStream tiffStream = new FileStream("output.tiff", FileMode.Create))
            {
                tiffRenderer.ToTiff(tiffStream);
            }
            Console.WriteLine("Rendered worksheet to TIFF format");

            // SaveFormat'ı XPS olarak değiştirin ve tekrar işleyin
            options.SaveFormat = SaveFormat.Xps;
            SheetRender xpsRenderer = new SheetRender(worksheet, options);
            using (FileStream xpsStream = new FileStream("output.xps", FileMode.Create))
            {
                // Not: SheetRender XPS formatını desteklemez. Bunun yerine görüntü formatı olarak kaydedilecektir.
                xpsRenderer.ToImage(0, xpsStream);
            }
            Console.WriteLine("Rendered worksheet to XPS format");
        }
    }
}
```

### Ayrıca Bakınız

* enum [SaveFormat](../../../aspose.cells/saveformat/)
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


