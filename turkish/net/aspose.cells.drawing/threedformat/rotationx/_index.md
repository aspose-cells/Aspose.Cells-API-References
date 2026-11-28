---
title: "ThreeDFormat.RotationX"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ThreeDFormat özelliği. Ekstrüde şeklin x ekseni etrafındaki dönüşünü derece cinsinden alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing/threedformat/rotationx/
---
## ThreeDFormat.RotationX property

Ekstrüde şeklin x ekseni etrafındaki dönüşünü derece cinsinden alır ve ayarlar.

```csharp
public double RotationX { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ThreeDFormatPropertyRotationXDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 3D biçimlendirmeyi göstermek için bir şekil ekle
            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 2, 2, 2, 200, 100, 100);
            
            // 3D formatını al (3D efektleri \"etkinleştirmeye\" gerek yok - sadece özellikleri ayarla)
            ThreeDFormat threeDFormat = shape.ThreeDFormat;

            // Mevcut RotationX değerini göster
            Console.WriteLine("Current RotationX value: " + threeDFormat.RotationX);

            // Yeni RotationX değerini ayarla (x ekseni etrafındaki dönüş derece cinsinden)
            threeDFormat.RotationX = 45;
            Console.WriteLine("New RotationX value: " + threeDFormat.RotationX);

            // Dönüşü görünür kılmak için diğer 3D özelliklerini ayarla
            threeDFormat.ExtrusionHeight = 20;
            threeDFormat.ContourWidth = 2;
            threeDFormat.PresetCameraType = PresetCameraType.OrthographicFront;

            // Etkileri görmek için çalışma kitabını kaydedin
            workbook.Save("ThreeDFormatRotationXDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


