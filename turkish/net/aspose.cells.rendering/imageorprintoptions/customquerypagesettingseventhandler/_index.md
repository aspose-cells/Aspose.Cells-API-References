---
title: "ImageOrPrintOptions.CustomQueryPageSettingsEventHandler"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ImageOrPrintOptions özelliği. İstemci, her sayfayı yazdırırken bu EventHandler'ı kullanarak yazıcının sayfa ayarlarını kontrol edebilir"
type: docs
url: /tr/net/aspose.cells.rendering/imageorprintoptions/customquerypagesettingseventhandler/
---
## ImageOrPrintOptions.CustomQueryPageSettingsEventHandler property

İstemci, bu EventHandler'ı kullanarak her sayfayı yazdırırken yazıcının sayfa ayarlarını kontrol edebilir.

```csharp
public QueryPageSettingsEventHandler CustomQueryPageSettingsEventHandler { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class ImageOrPrintOptionsPropertyCustomQueryPageSettingsEventHandlerDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri ekleyin
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B1"].Value = "More Data";

            try
            {
                // ImageOrPrintOptions örneği oluşturun
                ImageOrPrintOptions options = new ImageOrPrintOptions();

                // Mevcut özelliklerin bir kısmını göster
                Console.WriteLine("Current HorizontalResolution: " + options.HorizontalResolution);
                Console.WriteLine("Current VerticalResolution: " + options.VerticalResolution);
                Console.WriteLine("Current ImageType: " + options.ImageType);

                // Bazı özelliklerin ayarlanmasını göster
                options.HorizontalResolution = 300;
                options.VerticalResolution = 300;
                options.ImageType = Aspose.Cells.Drawing.ImageType.Png;

                // Özelliklerin ayarlandığını doğrula
                Console.WriteLine("Updated HorizontalResolution: " + options.HorizontalResolution);
                Console.WriteLine("Updated VerticalResolution: " + options.VerticalResolution);
                Console.WriteLine("Updated ImageType: " + options.ImageType);

                // Renderlemeyi göstermek için bir SheetRender oluştur
                SheetRender renderer = new SheetRender(worksheet, options);

                // Çalışma kitabını kaydedin
                workbook.Save("CustomQueryPageSettingsEventHandlerDemo.xlsx");

                Console.WriteLine("ImageOrPrintOptions demonstration completed");
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


