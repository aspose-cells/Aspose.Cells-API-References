---
title: "PictureBulletValue.ImageData"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PictureBulletValue özelliği. Merminin görüntü verisini alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing.texts/picturebulletvalue/imagedata/
---
## PictureBulletValue.ImageData property

Madde işaretinin görüntü verisini alır ve ayarlar.

```csharp
public byte[] ImageData { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;
    using System.IO;

    public class PictureBulletValuePropertyImageDataDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            try
            {
                // PictureBulletValue örneği oluştur
                PictureBulletValue bulletValue = new PictureBulletValue();
                
                // ImageData ayarlamayı ve almayı göster
                byte[] sampleImageData = new byte[] { 0x01, 0x02, 0x03 }; // Sample data
                bulletValue.ImageData = sampleImageData;
                
                // ImageData özelliği değerini göster
                Console.WriteLine("ImageData length: " + (bulletValue.ImageData?.Length ?? 0) + " bytes");
                
                // Type özelliğini göster (yalnızca okuma)
                Console.WriteLine("Bullet Type: " + bulletValue.Type);
                
                // Çalışma kitabını kaydedin
                workbook.Save("PictureBulletValueImageDataDemo.xlsx");
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

* class [PictureBulletValue](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


