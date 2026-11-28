---
title: "ThreeDFormat.RotationY"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ThreeDFormat özelliği. Çıkarılan şeklin y ekseni etrafındaki dönüşünü derece cinsinden alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing/threedformat/rotationy/
---
## ThreeDFormat.RotationY property

Ekstrüde şeklin y ekseni etrafındaki dönüşünü derece cinsinden alır ve ayarlar.

```csharp
public double RotationY { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ThreeDFormatPropertyRotationYDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 3D biçimlendirmeyi göstermek için bir şekil ekle
            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.TextBox, 2, 0, 2, 100, 150, 150);
            shape.Text = "3D Rotation Demo";
            
            // Şeklin ThreeDFormat'ına eriş
            ThreeDFormat threeDFormat = shape.ThreeDFormat;

            // Mevcut RotationY değerini göster
            Console.WriteLine("Current RotationY value: " + threeDFormat.RotationY);

            // Yeni RotationY değerleri ayarla ve etkileri göster
            threeDFormat.RotationY = 15;
            Console.WriteLine("Shape rotated 15 degrees around Y-axis");

            // Etkisinin görünür olmasını sağlamak için başka 3D özellikleri uygula
            threeDFormat.ExtrusionHeight = 5;
            threeDFormat.ContourWidth = 1;
            threeDFormat.PresetCameraType = PresetCameraType.PerspectiveContrastingRightFacing;

            // Etkileri göstermek için çalışma kitabını kaydet
            workbook.Save("ThreeDFormatRotationYDemo.xlsx");

            // Rotasyonu tekrar değiştir ve başka bir sürüm kaydet
            threeDFormat.RotationY = 45;
            workbook.Save("ThreeDFormatRotationYDemo_45degrees.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


