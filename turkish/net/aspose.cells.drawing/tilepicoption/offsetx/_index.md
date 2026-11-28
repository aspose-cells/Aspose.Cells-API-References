---
title: "TilePicOption.OffsetX"
second_title: "Aspose.Cells için .NET API Referansı"
description: "TilePicOption özelliği. Döşeme resmi için X kaydırmasını alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing/tilepicoption/offsetx/
---
## TilePicOption.OffsetX property

Döşeme resminin X ofsetini alır veya ayarlar.

```csharp
public double OffsetX { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class TilePicOptionPropertyOffsetXDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Döşemeyi göstermek için bir dikdörtgen şekil ekle
            Shape rectangle = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 200, 200);

            // Döşemeli resmi kullanmak için dolgu biçimini yapılandır
            FillFormat fillFormat = rectangle.Fill;
            fillFormat.FillType = FillType.Texture;

            // TilePicOption oluştur ve yapılandır
            TilePicOption tileOptions = new TilePicOption();
            
            // İlk OffsetX değerini oku
            Console.WriteLine("Current OffsetX value: " + tileOptions.OffsetX);

            // Döşeme deseni için yeni X kaydırmasını ayarla
            tileOptions.OffsetX = 15.5;

            // Döşeme seçeneklerini şekil dolgusuna uygula
            fillFormat.TextureFill.TilePicOption = tileOptions;

            // Minimum 1x1 piksel görüntüyü yükle (kırmızı nokta)
            byte[] imageData = Convert.FromBase64String(
                "iVBORw0KGgoAAAANSUhEUgAAAAEAAAABCAYAAAAfFcSJAAAADUlEQVR42mNkYPhfDwAChwGA60e6kgAAAABJRU5ErkJggg==");
            fillFormat.ImageData = imageData;

            // Değiştirilmiş çalışma kitabını kaydet
            workbook.Save("TilePicOptionPropertyOffsetXDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [TilePicOption](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


