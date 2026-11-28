---
title: "MarkdownSaveOptions.ImageOptions"
second_title: "Aspose.Cells için .NET API Referansı"
description: "MarkdownSaveOptions özelliği. Dışa aktarmadan önce ImageOrPrintOptions nesnesini al"
type: docs
url: /tr/net/aspose.cells/markdownsaveoptions/imageoptions/
---
## MarkdownSaveOptions.ImageOptions property

Dışa aktarmadan önce ImageOrPrintOptions nesnesini alın

```csharp
public ImageOrPrintOptions ImageOptions { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class MarkdownSaveOptionsPropertyImageOptionsDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // Örnek bir çalışma sayfası oluşturun
            Worksheet worksheet = workbook.Worksheets[0];

            // Örneği anlamlı kılmak için bazı veriler ekleyin
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["A2"].Value = "Image Options Demo";

            try
            {
                // MarkdownSaveOptions örneği oluştur
                MarkdownSaveOptions saveOptions = new MarkdownSaveOptions();

                // ImageOptions özelliğine eriş (yalnızca okunabilir)
                ImageOrPrintOptions imageOptions = saveOptions.ImageOptions;

                // ImageOptions özelliklerinin mevcut değerlerini göster
                Console.WriteLine("ImageOptions properties:");
                Console.WriteLine($"HorizontalResolution: {imageOptions.HorizontalResolution}");
                Console.WriteLine($"VerticalResolution: {imageOptions.VerticalResolution}");
                Console.WriteLine($"ImageType: {imageOptions.ImageType}");
                Console.WriteLine($"Quality: {imageOptions.Quality}");
                Console.WriteLine($"Transparent: {imageOptions.Transparent}");

                // Çalışma kitabını mevcut seçeneklerle kaydet
                workbook.Save("ImageOptionsDemo.md", saveOptions);

                Console.WriteLine("Markdown file saved successfully with ImageOptions demonstrated.");
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

* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions/)
* class [MarkdownSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


