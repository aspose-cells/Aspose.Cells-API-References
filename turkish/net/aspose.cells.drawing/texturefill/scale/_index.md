---
title: "TextureFill.Scale"
second_title: "Aspose.Cells için .NET API Referansı"
description: "TextureFill özelliği. Resim formatı ölçeğini alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing/texturefill/scale/
---
## TextureFill.Scale property

Resim formatı ölçeğini alır ve ayarlar.

```csharp
public double Scale { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class TextureFillPropertyScaleDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir şekil ekle ve doldurma biçimini al
            Shape shape = worksheet.Shapes.AddRectangle(0, 0, 10, 10, 500, 300);
            FillFormat fillFormat = shape.Fill;

            // Doku doldurmayı yapılandır
            fillFormat.FillType = FillType.Texture;
            TextureFill textureFill = fillFormat.TextureFill;

            // Doku görüntüsünü yükle ve özellikleri yapılandır
            textureFill.ImageData = File.ReadAllBytes("texture.jpg");
            textureFill.Type = TextureType.Unknown; // Changed from UserDefined to Unknown
            textureFill.IsTiling = true;

            // Ölçeği göster ve değiştir
            Console.WriteLine("Initial Scale: " + textureFill.Scale);
            textureFill.Scale = 0.5;
            Console.WriteLine("Modified Scale: " + textureFill.Scale);

            // Sonucu kaydedin
            workbook.Save("TextureFillScaleDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [TextureFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


