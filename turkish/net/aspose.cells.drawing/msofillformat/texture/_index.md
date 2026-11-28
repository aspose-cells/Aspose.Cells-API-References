---
title: "MsoFillFormat.Texture"
second_title: "Aspose.Cells için .NET API Referansı"
description: "MsoFillFormat özelliği. Doku doldurma tipini alır"
type: docs
url: /tr/net/aspose.cells.drawing/msofillformat/texture/
---
## MsoFillFormat.Texture property

Doku dolgu tipini alır.

```csharp
public TextureType Texture { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class MsoFillFormatPropertyTextureDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Dolgu biçimlendirmesini göstermek için bir dikdörtgen şekil ekle
            var rectangle = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 150, 200);

            // Dolgu formatını al
            MsoFillFormat fillFormat = rectangle.FillFormat;

            try
            {
                // Mevcut doku tipini göster (yalnızca okunabilir özellik)
                TextureType currentTexture = fillFormat.Texture;
                Console.WriteLine("Current Texture Type: " + currentTexture);

                // Doku değişebileceği için bazı görüntü verilerini ayarla
                // Bu, dokunun görüntü verileri tarafından nasıl etkilenebileceğini gösterir
                byte[] sampleImageData = new byte[] { 0x89, 0x50, 0x4E, 0x47 }; // PNG header
                fillFormat.ImageData = sampleImageData;

                // Görüntü verileri ayarlandıktan sonra doku tipini tekrar göster
                TextureType updatedTexture = fillFormat.Texture;
                Console.WriteLine("Texture Type after setting image data: " + updatedTexture);

                // Çalışma kitabını kaydedin
                workbook.Save("TextureDemo.xlsx");
                Console.WriteLine("Texture demonstration completed successfully.");
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

* enum [TextureType](../../texturetype/)
* class [MsoFillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


