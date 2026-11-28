---
title: "ThreeDFormat.Lighting"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ThreeDFormat özelliği. Işık setinin tipini alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing/threedformat/lighting/
---
## ThreeDFormat.Lighting property

Işık düzeninin tipini alır ve ayarlar.

```csharp
public LightRigType Lighting { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ThreeDFormatPropertyLightingDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 3D biçimlendirmeyi göstermek için bir şekil ekle
            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.TextBox, 1, 1, 0, 0, 200, 200);
            shape.Text = "3D Lighting Demo";
            
            // Şeklin ThreeDFormat'ını al
            ThreeDFormat threeDFormat = shape.ThreeDFormat;

            // Mevcut aydınlatma değerini göster
            Console.WriteLine("Current Lighting value: " + threeDFormat.Lighting);

            // Farklı aydınlatma tiplerini ayarla ve etkileri gözlemle
            threeDFormat.Lighting = LightRigType.BrightRoom;
            Console.WriteLine("Changed to BrightRoom lighting");

            // Aydınlatma etkisini daha iyi görmek için başka 3D özellikler uygula
            threeDFormat.TopBevelType = BevelType.ArtDeco;
            threeDFormat.TopBevelWidth = 10;
            threeDFormat.TopBevelHeight = 10;
            threeDFormat.ExtrusionHeight = 20;
            threeDFormat.ContourWidth = 2;
            threeDFormat.PresetCameraType = PresetCameraType.PerspectiveFront;

            // İlk aydınlatma tipiyle kaydet
            workbook.Save("BrightRoomLighting.xlsx");

            // Başka bir aydınlatma tipine değiştir
            threeDFormat.Lighting = LightRigType.Sunset;
            Console.WriteLine("Changed to Sunset lighting");
            workbook.Save("SunsetLighting.xlsx");

            // Üçüncü bir aydınlatma tipine değiştir
            threeDFormat.Lighting = LightRigType.ThreePoint;
            Console.WriteLine("Changed to ThreePoint lighting");
            workbook.Save("ThreePointLighting.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [LightRigType](../../lightrigtype/)
* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


