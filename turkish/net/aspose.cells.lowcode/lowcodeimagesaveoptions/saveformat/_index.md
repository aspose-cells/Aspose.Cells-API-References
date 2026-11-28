---
title: "LowCodeImageSaveOptions.SaveFormat"
second_title: "Aspose.Cells için .NET API Referansı"
description: "LowCodeImageSaveOptions özelliği. Kaydetme formatını alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells.lowcode/lowcodeimagesaveoptions/saveformat/
---
## LowCodeImageSaveOptions.SaveFormat property

Kaydetme biçimini alır veya ayarlar.

```csharp
public override SaveFormat SaveFormat { get; set; }
```

### Açıklamalar

Eğer [`ImageOptions`](../imageoptions/) belirtilmişse, bu özelliği ayarlamak aynı zamanda [`ImageType`](../../../aspose.cells.rendering/imageorprintoptions/imagetype/) değerini de değiştirecektir.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.LowCode;
    using Aspose.Cells.Rendering;
    using System;

    public class LowCodeImageSaveOptionsPropertySaveFormatDemo
    {
        public static void Run()
        {
            // Örnek verilerle yeni bir çalışma kitabı oluşturun
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Aspose.Cells LowCode Image SaveFormat Demo");

            // LowCodeImageSaveOptions'ı varsayılan değerlerle başlat
            LowCodeImageSaveOptions options = new LowCodeImageSaveOptions();
            
            // İlk SaveFormat'ı göster (varsayılan Png'dir)
            Console.WriteLine("Initial SaveFormat: " + options.SaveFormat);

            // JPEG çıktısı için yapılandır
            options.SaveFormat = SaveFormat.Jpg;
            options.ImageOptions = new ImageOrPrintOptions
            {
                Quality = 85,
                OnePagePerSheet = true,
                ImageType = ImageType.Jpeg
            };
            SaveWorksheetAsImage(worksheet, options, "output_initial.jpg");

            // PNG formatına değiştir ve tekrar kaydet
            options.SaveFormat = SaveFormat.Png;
            options.ImageOptions.ImageType = ImageType.Png;
            Console.WriteLine("\nModified SaveFormat: " + options.SaveFormat);
            SaveWorksheetAsImage(worksheet, options, "output_modified.png");
        }

        private static void SaveWorksheetAsImage(Worksheet worksheet, LowCodeImageSaveOptions options, string fileName)
        {
            // Yapılandırılmış seçenekleri kullanarak çalışma sayfasını renderla
            SheetRender renderer = new SheetRender(worksheet, options.ImageOptions);
            renderer.ToImage(0, fileName);
            Console.WriteLine($"Saved: {fileName}");
        }
    }
}
```

### Ayrıca Bakınız

* enum [SaveFormat](../../../aspose.cells/saveformat/)
* class [LowCodeImageSaveOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


