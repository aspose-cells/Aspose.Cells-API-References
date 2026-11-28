---
title: "ImageOrPrintOptions.WarningCallback"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ImageOrPrintOptions özelliği. Uyarı geri çağrısını alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells.rendering/imageorprintoptions/warningcallback/
---
## ImageOrPrintOptions.WarningCallback property

Uyarı geri çağrısını alır veya ayarlar.

```csharp
public IWarningCallback WarningCallback { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class ImageOrPrintOptionsPropertyWarningCallbackDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluşturun ve ilk çalışma sayfasına erişin
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Renderleme sırasında bir uyarı oluşturacak içerik ekleyin
            worksheet.Cells["A1"].PutValue("This text uses a non-existent font");
            Style style = workbook.CreateStyle();
            style.Font.Name = "NonExistentFont";
            worksheet.Cells["A1"].SetStyle(style);

            // ImageOrPrintOptions örneği oluşturun
            ImageOrPrintOptions options = new ImageOrPrintOptions();

            // İlk WarningCallback değerini göster
            Console.WriteLine("Current WarningCallback value: " + options.WarningCallback);

            // Özel uyarı geri çağrısını oluşturun ve atayın
            var warningCallback = new RenderingWarningCallback();
            options.WarningCallback = warningCallback;

            // Renderleme sırasında geri çağrıyı göstermek için SheetRender oluşturun
            SheetRender renderer = new SheetRender(worksheet, options);
            renderer.ToImage(0, "output_image.png");

            // Uyarıların yakalanıp yakalanmadığını kontrol edin
            Console.WriteLine($"Total warnings captured: {warningCallback.WarningCount}");
        }
    }

    // Renderleme uyarılarını işlemek için özel geri çağrı uygulaması
    public class RenderingWarningCallback : IWarningCallback
    {
        public int WarningCount { get; private set; }

        public void Warning(WarningInfo warningInfo)
        {
            // Yazı tipi ikame uyarılarını işleyin
            if (warningInfo.WarningType == WarningType.FontSubstitution)
            {
                Console.WriteLine($"Font substitution warning: {warningInfo.Description}");
                WarningCount++;
            }
        }
    }
}
```

### Ayrıca Bakınız

* interface [IWarningCallback](../../../aspose.cells/iwarningcallback/)
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


