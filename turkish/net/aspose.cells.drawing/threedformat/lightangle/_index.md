---
title: "ThreeDFormat.LightAngle"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ThreeDFormat özelliği. Ekstrüzyon ışıklarının açısını alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing/threedformat/lightangle/
---
## ThreeDFormat.LightAngle property

Ekstrüzyon ışıklarının açısını alır ve ayarlar.

```csharp
public double LightAngle { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ThreeDFormatPropertyLightAngleDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 3D biçimlendirmeyi göstermek için bir şekil ekle
            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.TextBox, 1, 1, 200, 100, 0, 0);
            shape.Text = "3D Format Demo";
            
            // Şeklin ThreeDFormat'ına eriş
            ThreeDFormat threeDFormat = shape.ThreeDFormat;

            // Mevcut LightAngle değerini göster
            Console.WriteLine("Current LightAngle value: " + threeDFormat.LightAngle);

            // Yeni LightAngle değerini ayarla (0 ile 359,9 derece arasında)
            threeDFormat.LightAngle = 45;
            Console.WriteLine("New LightAngle value: " + threeDFormat.LightAngle);

            // LightAngle etkisini görmek için diğer 3D özelliklerini yapılandır
            threeDFormat.TopBevelType = BevelType.ArtDeco;
            threeDFormat.TopBevelWidth = 10;
            threeDFormat.TopBevelHeight = 10;
            threeDFormat.Material = PresetMaterialType.Plastic;
            threeDFormat.Lighting = LightRigType.ThreePoint;
            threeDFormat.LightingDirection = LightRigDirectionType.Top;

            // Etkileri görmek için çalışma kitabını kaydedin
            workbook.Save("ThreeDFormatLightAngleDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


