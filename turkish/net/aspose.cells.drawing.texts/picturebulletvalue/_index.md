---
title: "Sınıf PictureBulletValue"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Drawing.Texts.PictureBulletValue sınıfı. Görüntü madde işaretinin değerini temsil eder"
type: docs
url: /tr/net/aspose.cells.drawing.texts/picturebulletvalue/
---
## PictureBulletValue class

Görüntü madde işaretinin değerinin temsilidir.

```csharp
public class PictureBulletValue : BulletValue
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [PictureBulletValue](picturebulletvalue/)() | Varsayılan yapıcı. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [ImageData](../../aspose.cells.drawing.texts/picturebulletvalue/imagedata/) { get; set; } | Madde işaretinin görüntü verisini alır ve ayarlar. |
| override [Type](../../aspose.cells.drawing.texts/picturebulletvalue/type/) { get; } | Madde işaretinin değerinin tipini alır. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;
    using System.IO;

    public class TextsClassPictureBulletValueDemo
    {
        public static void Run()
        {
            // Demonstrasyon için yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            try
            {
                // PictureBulletValue sınıfının bir örneğini oluştur
                PictureBulletValue bulletValue = new PictureBulletValue();
                
                // Örnek görüntü verisini yükle (gerçek görüntü yoluyla değiştir)
                string imagePath = "sample.png";
                if (File.Exists(imagePath))
                {
                    bulletValue.ImageData = File.ReadAllBytes(imagePath);
                    
                    // Temel bilgileri göster
                    Console.WriteLine($"PictureBulletValue created with Type: {bulletValue.Type}");
                    Console.WriteLine($"Image data length: {bulletValue.ImageData?.Length ?? 0} bytes");
                }
                else
                {
                    Console.WriteLine("Sample image not found, using empty bullet value");
                }
                
                // Çalışma kitabını kaydedin
                workbook.Save("PictureBulletValueDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with PictureBulletValue: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [BulletValue](../bulletvalue/)
* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)


