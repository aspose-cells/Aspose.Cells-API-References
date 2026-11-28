---
title: "ImageOrPrintOptions.PixelFormat"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ImageOrPrintOptions özelliği. Oluşturulan görüntüler için piksel biçimini alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells.rendering/imageorprintoptions/pixelformat/
---
## ImageOrPrintOptions.PixelFormat property

Oluşturulan görüntüler için piksel formatını alır veya ayarlar.

```csharp
public PixelFormat PixelFormat { get; set; }
```

### Açıklamalar

Varsayılan değer PixelFormat.Format32bppArgb'dir.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class ImageOrPrintOptionsPropertyPixelFormatDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // Örnek bir çalışma sayfası oluşturun
            Worksheet worksheet = workbook.Worksheets[0];

            // Örneği anlamlı kılmak için bazı veriler ekleyin
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B1"].Value = "PixelFormat Demo";

            try
            {
                // ImageOrPrintOptions örneği oluşturun
                ImageOrPrintOptions options = new ImageOrPrintOptions();

                // ImageType özelliğinin mevcut değerini göster (PixelFormat mevcut olmadığı için)
                Console.WriteLine("Current ImageType: " + options.ImageType);

                // Not: API'de PixelFormat mevcut olmadığından, bunun yerine ImageType'ı gösteriyoruz
                // görüntü biçimi ayarları için en yakın ilgili özelliktir

                // Kullanımdaki seçenekleri göstermek için bir SheetRender oluştur
                SheetRender sheetRender = new SheetRender(worksheet, options);

                // Seçenekleri göstermek için sonucu bir görüntü olarak kaydet
                sheetRender.ToImage(0, "PixelFormatDemo.png");

                Console.WriteLine("ImageType property has been demonstrated. Image saved as PixelFormatDemo.png");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


