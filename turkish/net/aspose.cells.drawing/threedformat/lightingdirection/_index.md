---
title: "ThreeDFormat.LightingDirection"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ThreeDFormat özelliği. Işık setinin sahneye göre yönlendirildiği yönü alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing/threedformat/lightingdirection/
---
## ThreeDFormat.LightingDirection property

Işık düzeninin sahneyle ilişkili olarak yönlendirildiği yönü alır ve ayarlar.

```csharp
public LightRigDirectionType LightingDirection { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ThreeDFormatPropertyLightingDirectionDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 3D biçimlendirmeyi göstermek için bir şekil ekle
            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.TextBox, 1, 1, 0, 0, 200, 100);
            shape.Text = "3D Lighting Direction Demo";
            
            // Şeklin ThreeDFormat'ını al
            ThreeDFormat threeDFormat = shape.ThreeDFormat;

            // İlk 3D özelliklerini ayarla
            threeDFormat.TopBevelType = BevelType.ArtDeco;
            threeDFormat.TopBevelWidth = 10;
            threeDFormat.TopBevelHeight = 10;
            threeDFormat.ExtrusionHeight = 20;
            threeDFormat.ContourWidth = 2;
            threeDFormat.Lighting = LightRigType.ThreePoint;
            threeDFormat.Material = PresetMaterialType.Plastic;

            // Mevcut aydınlatma yönünü göster
            Console.WriteLine("Current LightingDirection: " + threeDFormat.LightingDirection);

            // Aydınlatma yönünü değiştir ve etkileri gözlemle
            threeDFormat.LightingDirection = LightRigDirectionType.TopLeft;
            Console.WriteLine("Changed LightingDirection to TopLeft");

            // Başka bir yöne değiştir
            threeDFormat.LightingDirection = LightRigDirectionType.BottomRight;
            Console.WriteLine("Changed LightingDirection to BottomRight");

            // Görsel etkileri görmek için çalışma kitabını kaydet
            workbook.Save("ThreeDFormatLightingDirectionDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [LightRigDirectionType](../../lightrigdirectiontype/)
* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


