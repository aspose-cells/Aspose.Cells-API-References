---
title: "DrawObject.ImageBytes"
second_title: "Aspose.Cells için .NET API Referansı"
description: "DrawObject özelliği. Render sırasında oluşturulan Grafik Şeklinin görüntü baytlarını gösterir"
type: docs
url: /tr/net/aspose.cells.rendering/drawobject/imagebytes/
---
## DrawObject.ImageBytes property

Render edilen Chart, Shape'in görüntü baytlarını gösterir.

```csharp
public byte[] ImageBytes { get; }
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

    public class DrawObjectPropertyImageBytesDemo
    {
        // Görüntü baytlarını yakalamak için özel olay işleyicisi
        private class ImageBytesHandler : DrawObjectEventHandler
        {
            public byte[] CapturedImageBytes { get; private set; }

            public override void Draw(DrawObject drawObject, float x, float y, float width, float height)
            {
                if (drawObject.Type == DrawObjectEnum.Image)
                {
                    CapturedImageBytes = drawObject.ImageBytes;
                    Console.WriteLine($"Captured image size: {CapturedImageBytes?.Length ?? 0} bytes");
                }
            }
        }

        public static void Run()
        {
            // Yeni bir çalışma kitabı oluşturun ve ilk çalışma sayfasına erişin
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Base64 kodlu 1x1 kırmızı piksel PNG
            byte[] generatedImageBytes = Convert.FromBase64String("iVBORw0KGgoAAAANSUhEUgAAAAEAAAABCAYAAAAfFcSJAAAADUlEQVR42mNkYPhfDwAChwGA60e6kgAAAABJRU5ErkJggg==");

            // Oluşturulan görüntüyü bir akış kullanarak çalışma sayfasına ekleyin
            using (MemoryStream imageStream = new MemoryStream(generatedImageBytes))
            {
                worksheet.Pictures.Add(0, 0, imageStream);
            }

            // Render seçeneklerini ayarlayın
            ImageOrPrintOptions renderOptions = new ImageOrPrintOptions();
            renderOptions.ImageType = ImageType.Png;

            // İşleyici örneğini oluşturun ve seçeneklere atayın
            var imageHandler = new ImageBytesHandler();
            renderOptions.DrawObjectEventHandler = imageHandler;

            SheetRender sheetRenderer = new SheetRender(worksheet, renderOptions);
            
            // Sahte bir akış kullanarak DrawObject olayını tetiklemek için çalışma sayfasını render edin
            using (MemoryStream dummyStream = new MemoryStream())
            {
                sheetRenderer.ToImage(0, dummyStream);
            }

            // Eğer mevcutsa yakalanan görüntüyü çalışma sayfasına ekleyin
            byte[] capturedImageBytes = imageHandler.CapturedImageBytes;
            if (capturedImageBytes != null)
            {
                int newRowPosition = worksheet.Cells.MaxDataRow + 2;
                using (MemoryStream capturedStream = new MemoryStream(capturedImageBytes))
                {
                    worksheet.Pictures.Add(newRowPosition, 0, capturedStream);
                }
            }

            // Değiştirilmiş çalışma kitabını kaydet
            workbook.Save("ImageBytesDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [DrawObject](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


