---
title: "ThreeDFormat.RotationZ"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ThreeDFormat özelliği. Ekstrüde şeklin z ekseni etrafındaki dönüşünü derece cinsinden alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing/threedformat/rotationz/
---
## ThreeDFormat.RotationZ property

Ekstrüde şeklin z ekseni etrafındaki dönüşünü derece cinsinden alır ve ayarlar.

```csharp
public double RotationZ { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ThreeDFormatPropertyRotationZDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 3D biçimlendirmeyi göstermek için bir şekil ekle
            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.TextBox, 2, 0, 2, 0, 100, 150);
            shape.Text = "3D Rotation Demo";
            
            // Şeklin ThreeDFormat'ına eriş
            ThreeDFormat threeDFormat = shape.ThreeDFormat;

            // Mevcut RotationZ değerini göster
            Console.WriteLine("Current RotationZ value: " + threeDFormat.RotationZ);

            // Yeni RotationZ değerlerini ayarla ve etkileri göster
            threeDFormat.RotationZ = 45;
            Console.WriteLine("Shape rotated 45 degrees around Z-axis");

            // Dönüşü görünür kılmak için diğer 3D özelliklerini uygula
            threeDFormat.ExtrusionHeight = 15;
            threeDFormat.ContourWidth = 2;
            threeDFormat.PresetCameraType = PresetCameraType.OrthographicFront;

            // Çalışma kitabını 3D efektlerle kaydet
            workbook.Save("ThreeDFormatRotationZDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


