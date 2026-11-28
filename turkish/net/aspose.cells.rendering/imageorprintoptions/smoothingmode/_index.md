---
title: "ImageOrPrintOptions.SmoothingMode"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ImageOrPrintOptions özelliği. Çizgilere, eğrilere ve doldurulmuş alanların kenarlarına yumuşatma (antialiasing) uygulanıp uygulanmayacağını belirtir. Varsayılan değer SmoothingMode.None'dur."
type: docs
url: /tr/net/aspose.cells.rendering/imageorprintoptions/smoothingmode/
---
## ImageOrPrintOptions.SmoothingMode property

Düzleştirme (antialiasing) işleminin çizgilere, eğrilere ve doldurulmuş alanların kenarlarına uygulanıp uygulanmayacağını belirtir. Varsayılan değer SmoothingMode.None'dur.

```csharp
public SmoothingMode SmoothingMode { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;
    using System.IO;

    public class ImageOrPrintOptionsPropertySmoothingModeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri ekleyin
            worksheet.Cells["A1"].Value = "ImageOrPrintOptions Demo";
            worksheet.Cells["A2"].Value = "Sample Data";

            try
            {
                // ImageOrPrintOptions örneği oluşturun
                ImageOrPrintOptions options = new ImageOrPrintOptions();

                // Mevcut özelliklerin bir kısmını göster
                Console.WriteLine("HorizontalResolution: " + options.HorizontalResolution);
                Console.WriteLine("VerticalResolution: " + options.VerticalResolution);
                Console.WriteLine("ImageType: " + options.ImageType);

                // Özelliği göstermek için bir SheetRender oluşturun
                SheetRender renderer = new SheetRender(worksheet, options);

                // Fonksiyonelliği göstermek için bir bellek akışına render edin
                MemoryStream stream = new MemoryStream();
                renderer.ToImage(0, stream);

                Console.WriteLine("Sheet rendered successfully");
                Console.WriteLine("Image size: " + stream.Length + " bytes");

                // Çalışma kitabını kaydedin
                workbook.Save("ImageOrPrintOptionsDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
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


