---
title: "ThreeDFormat.Z"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ThreeDFormat özelliği. 3D şeklin yerden uzaklığını tanımlar"
type: docs
url: /tr/net/aspose.cells.drawing/threedformat/z/
---
## ThreeDFormat.Z property

3B şekil için yerden mesafeyi tanımlar.

```csharp
public double Z { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ThreeDFormatPropertyZDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 3D biçimlendirmeyi göstermek için bir şekil ekle
            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 1, 1, 0, 0, 200, 100);
            
            // Şeklin ThreeDFormat'ına eriş
            ThreeDFormat threeDFormat = shape.ThreeDFormat;

            // Mevcut Z değerini göster (yerden uzaklık)
            Console.WriteLine("Current Z value: " + threeDFormat.Z);

            // Şekli yerden daha uzağa taşımak için yeni Z değerini ayarla
            threeDFormat.Z = 20;
            Console.WriteLine("New Z value: " + threeDFormat.Z);

            // Etkiyi görünür kılmak için diğer 3D özelliklerini yapılandır
            threeDFormat.ExtrusionHeight = 30;
            threeDFormat.ContourWidth = 2;
            threeDFormat.PresetCameraType = PresetCameraType.PerspectiveContrastingRightFacing;

            // 3D efekti görmek için çalışma kitabını kaydet
            workbook.Save("ThreeDFormatPropertyZDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


