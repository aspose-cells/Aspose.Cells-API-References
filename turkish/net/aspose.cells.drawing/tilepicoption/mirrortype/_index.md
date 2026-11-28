---
title: "TilePicOption.MirrorType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "TilePicOption özelliği. Döşeme için yansıtma tipini alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing/tilepicoption/mirrortype/
---
## TilePicOption.MirrorType property

Döşeme için ayna tipini alır veya ayarlar.

```csharp
public MirrorType MirrorType { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class TilePicOptionPropertyMirrorTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Gerekli tüm parametrelerle bir dikdörtgen şekil ekle
            Shape shape = worksheet.Shapes.AddRectangle(0, 0, 0, 500, 500, 500);

            // Örnek görüntü verisini yükle (gerçek görüntü yoluyla değiştir)
            byte[] imageData = File.ReadAllBytes("sample.png");

            // TilePicOption örneği oluştur ve yapılandır
            TilePicOption tileOptions = new TilePicOption();

            // İlk MirrorType değerini göster
            Console.WriteLine("Current MirrorType: " + tileOptions.MirrorType);

            // Döşeme seçeneklerini yapılandır.
            tileOptions.ScaleX = 0.5;
            tileOptions.ScaleY = 0.5;
            tileOptions.MirrorType = MirrorType.Both;

            // Doğru özellikleri kullanarak döşeme yapılandırmasını uygula
            shape.Fill.FillType = FillType.Texture;
            shape.Fill.ImageData = imageData;
            shape.Fill.TextureFill.TilePicOption = tileOptions;

            // Değiştirilmiş çalışma kitabını kaydet
            workbook.Save("TilePicOptionMirrorTypeDemo.xlsx");

            Console.WriteLine("Updated MirrorType: " + tileOptions.MirrorType);
        }
    }
}
```

### Ayrıca Bakınız

* enum [MirrorType](../../mirrortype/)
* class [TilePicOption](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


