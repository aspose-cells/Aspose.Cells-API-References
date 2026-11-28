---
title: "TextureFill.Transparency"
second_title: "Aspose.Cells için .NET API Referansı"
description: "TextureFill özelliği. Alanın şeffaflık derecesini 0.0 opak'tan 1.0 tamamen şeffaf'a kadar bir değer olarak döndürür veya ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing/texturefill/transparency/
---
## TextureFill.Transparency property

Alan şeffaflık derecesini 0.0 (opak) ile 1.0 (şeffaf) arasında bir değer olarak döndürür veya ayarlar.

```csharp
public double Transparency { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class TextureFillPropertyTransparencyDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına bir dikdörtgen şekli ekle
            Shape shape = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 100, 200);

            // Dolgu tipini doku olarak ayarla
            shape.Fill.FillType = FillType.Texture;

            // TextureFill özelliklerine eriş
            TextureFill textureFill = shape.Fill.TextureFill;

            // Yerleşik bir doku tipini ayarla
            textureFill.Type = TextureType.BlueTissuePaper;

            // İlk şeffaflık değerini göster
            Console.WriteLine("Initial Transparency: " + textureFill.Transparency);

            // Şeffaflığı %70'e değiştir (0.0 = opak, 1.0 = tamamen şeffaf)
            textureFill.Transparency = 0.7;
            Console.WriteLine("Updated Transparency: " + textureFill.Transparency);

            // Görünür şeffaflık etkisiyle çalışma kitabını kaydet
            workbook.Save("TextureFillTransparencyDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [TextureFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


