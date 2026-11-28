---
title: "TilePicOption.AlignmentType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "TilePicOption özelliği. Döşeme hizalamasını alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing/tilepicoption/alignmenttype/
---
## TilePicOption.AlignmentType property

Döşeme hizalamasını alır veya ayarlar.

```csharp
public RectangleAlignmentType AlignmentType { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class TilePicOptionPropertyAlignmentTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Döşemeyi göstermek için bir dikdörtgen şekil ekle
            Shape rectangle = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 300, 300);

            // Döşemeli resmi kullanmak için dolgu biçimini yapılandır
            FillFormat fillFormat = rectangle.Fill;
            fillFormat.FillType = FillType.Texture;

            // TilePicOption oluştur ve yapılandır
            TilePicOption tileOptions = new TilePicOption();
            
            // İlk AlignmentType değerini göster
            Console.WriteLine("Current AlignmentType: " + tileOptions.AlignmentType);

            // Hizalamayı ÜstSağ olarak ayarla
            tileOptions.AlignmentType = RectangleAlignmentType.TopRight;
            tileOptions.ScaleX = 0.5;
            tileOptions.ScaleY = 0.5;

            // Döşeme seçeneklerini şekil dolgusuna uygula
            fillFormat.TextureFill.TilePicOption = tileOptions;

            // Örnek resmi yükle (1x1 piksel kırmızı nokta)
            byte[] imageData = Convert.FromBase64String(
                "iVBORw0KGgoAAAANSUhEUgAAAAEAAAABCAYAAAAfFcSJAAAADUlEQVR42mNkYPhfDwAChwGA60e6kgAAAABJRU5ErkJggg==");
            fillFormat.ImageData = imageData;

            // Değiştirilmiş çalışma kitabını kaydet
            workbook.Save("TilePicOptionPropertyAlignmentTypeDemo.xlsx");

            // Hizalamayı AltSol olarak değiştir ve başka bir sürüm kaydet
            tileOptions.AlignmentType = RectangleAlignmentType.BottomLeft;
            workbook.Save("TilePicOptionPropertyAlignmentTypeDemo_BottomLeft.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [RectangleAlignmentType](../../rectanglealignmenttype/)
* class [TilePicOption](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


