---
title: "TextureFill.Type"
second_title: "Aspose.Cells için .NET API Referansı"
description: "TextureFill özelliği. Doku tipini alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing/texturefill/type/
---
## TextureFill.Type property

Doku tipini alır ve ayarlar.

```csharp
public TextureType Type { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class TextureFillPropertyTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Doku doldurmayı göstermek için bir dikdörtgen şekil ekle.
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 200);

            // Dolgu tipini doku olarak ayarla
            shape.Fill.FillType = FillType.Texture;

            // TextureFill özelliklerine eriş
            TextureFill textureFill = shape.Fill.TextureFill;

            try
            {
                // İlk Type değerini göster
                Console.WriteLine("Initial Texture Type: " + textureFill.Type);

                // Farklı bir doku tipi ayarla
                textureFill.Type = TextureType.Granite;
                Console.WriteLine("Updated Texture Type: " + textureFill.Type);

                // Başka bir doku tipini göster
                textureFill.Type = TextureType.WaterDroplets;
                Console.WriteLine("Final Texture Type: " + textureFill.Type);

                // Etkiyi görmek için çalışma kitabını kaydet
                workbook.Save("TextureFillTypeDemo.xlsx");
                Console.WriteLine("Texture fill type demonstration completed successfully.");
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
* class [TextureFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


