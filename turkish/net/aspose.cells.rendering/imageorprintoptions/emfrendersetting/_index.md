---
title: "ImageOrPrintOptions.EmfRenderSetting"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ImageOrPrintOptions özelliği. Kaynak dosyada EMF metafile'larını renderlemek için ayar"
type: docs
url: /tr/net/aspose.cells.rendering/imageorprintoptions/emfrendersetting/
---
## ImageOrPrintOptions.EmfRenderSetting property

Kaynak dosyada Emf metafile'lerinin render edilmesi için ayar.

```csharp
public EmfRenderSetting EmfRenderSetting { get; set; }
```

### Açıklamalar

"EMF+ Dual" olarak tanımlanan EMF metafile'ları hem EMF+ kayıtlarını hem de EMF kayıtlarını içerebilir. Görüntüyü renderlemek için her iki kayıt türü de, yalnızca EMF+ kayıtları veya yalnızca EMF kayıtları kullanılabilir. EmfPlusPrefer ayarlandığında, görüntüye renderleme sırasında EMF+ kayıtları ayrıştırılır, aksi takdirde yalnızca EMF kayıtları ayrıştırılır. Varsayılan değer EmfOnly'dur. .NET System.Drawing.Common'a bağımlı çerçeveler için bu ayar göz ardı edilir.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing; // Added missing namespace AsposeCellsExamples
    using Aspose.Cells.Rendering;
    using System;

    public class ImageOrPrintOptionsPropertyEmfRenderSettingDemo
    {
        public static void Run()
        {
            // Test içeriğiyle yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "EMF Rendering Setting Test";
            worksheet.Cells["C5"].Value = "Sample Content for Image Rendering";

            // Görüntü renderleme seçeneklerini oluştur
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = ImageType.Tiff;
            options.TiffCompression = TiffCompression.CompressionLZW;

            // Mevcut ayarı göster
            Console.WriteLine("Default EmfRenderSetting: " + options.EmfRenderSetting);

            // Varsayılan EMF ayarlarıyla renderle
            SheetRender renderer = new SheetRender(worksheet, options);
            renderer.ToImage(0, "DefaultEmfSetting.tiff");

            // EMF render ayarını değiştirin ve tekrar render edin
            options.EmfRenderSetting = EmfRenderSetting.EmfPlusPrefer;
            Console.WriteLine("\nModified EmfRenderSetting: " + options.EmfRenderSetting);

            SheetRender modifiedRenderer = new SheetRender(worksheet, options);
            modifiedRenderer.ToImage(0, "ModifiedEmfSetting.tiff");

            Console.WriteLine("\nGenerated TIFF images demonstrating EMF rendering settings.");
        }
    }
}
```

### Ayrıca Bakınız

* enum [EmfRenderSetting](../../../aspose.cells/emfrendersetting/)
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


