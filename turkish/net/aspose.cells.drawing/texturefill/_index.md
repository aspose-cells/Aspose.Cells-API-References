---
title: "Sınıf TextureFill"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Drawing.TextureFill sınıfı. Doku dolgu formatını temsil eden nesneyi kapsüller"
type: docs
url: /tr/net/aspose.cells.drawing/texturefill/
---
## TextureFill class

Doku dolgu biçimini temsil eden nesneyi kapsüller

```csharp
public class TextureFill : Fill
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [ImageData](../../aspose.cells.drawing/texturefill/imagedata/) { get; set; } | Dolgunun görüntü verisini alır ve ayarlar. |
| [IsTiling](../../aspose.cells.drawing/texturefill/istiling/) { get; set; } | Resmin doku olarak döşenip döşenmediğini gösterir. |
| [PicFormatOption](../../aspose.cells.drawing/texturefill/picformatoption/) { get; set; } | Resim formatı seçeneğini alır veya ayarlar. |
| [PictureFormatType](../../aspose.cells.drawing/texturefill/pictureformattype/) { get; set; } | Resim formatı tipini alır ve ayarlar. |
| [Scale](../../aspose.cells.drawing/texturefill/scale/) { get; set; } | Resim formatı ölçeğini alır ve ayarlar. |
| [TilePicOption](../../aspose.cells.drawing/texturefill/tilepicoption/) { get; set; } | Döşeme resim seçeneğini alır veya ayarlar. |
| [Transparency](../../aspose.cells.drawing/texturefill/transparency/) { get; set; } | Alan şeffaflık derecesini 0.0 (opak) ile 1.0 (şeffaf) arasında bir değer olarak döndürür veya ayarlar. |
| [Type](../../aspose.cells.drawing/texturefill/type/) { get; set; } | Doku tipini alır ve ayarlar. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| override [Equals](../../aspose.cells.drawing/fill/equals/)(object) | /(Şuradan [`Fill`](../fill/) devralınmıştır.) |
| override [GetHashCode](../../aspose.cells.drawing/fill/gethashcode/)() | Karma kodu alır. (Şuradan [`Fill`](../fill/) devralınmıştır.) |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class DrawingClassTextureFillDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Doku doldurmayı göstermek için bir dikdörtgen şekil ekle.
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 150, 300);
            
            // Şekle doku doldurmayı uygula ve mevcut TextureFill örneğini al.
            shape.Fill.FillType = FillType.Texture;
            TextureFill textureFill = shape.Fill.TextureFill;
            
            // Yerleşik doku tipini ayarla.
            textureFill.Type = TextureType.BlueTissuePaper;
            
            // Döşeme seçeneklerini yapılandır.
            textureFill.IsTiling = true;
            TilePicOption tileOptions = new TilePicOption
            {
                ScaleX = 0.5,
                ScaleY = 0.5,
                OffsetX = 10,
                OffsetY = 10
            };
            textureFill.TilePicOption = tileOptions;
            
            // Doldurma şeffaflığını ve ölçeklemeyi ayarla.
            textureFill.Transparency = 0.2;
            textureFill.Scale = 0.8;
            
            // Doku doldurması uygulanmış çalışma kitabını kaydet.
            workbook.Save("TextureFillDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Fill](../fill/)
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


