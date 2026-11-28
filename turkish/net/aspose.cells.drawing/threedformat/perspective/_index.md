---
title: "ThreeDFormat.Perspective"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ThreeDFormat özelliği. Bir ThreeDFormat nesnesinin görüntülenebileceği açıyı alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing/threedformat/perspective/
---
## ThreeDFormat.Perspective property

Bir ThreeDFormat nesnesinin görüntülenebileceği açıyı alır ve ayarlar.

```csharp
public double Perspective { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ThreeDFormatPropertyPerspectiveDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 3D biçimlendirmeyi göstermek için bir şekil ekle
            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 0, 0, 0, 0, 200, 100);
            
            // Şeklin 3D biçimini al
            ThreeDFormat threeDFormat = shape.ThreeDFormat;

            // Mevcut perspektif değerini göster
            Console.WriteLine("Current Perspective value: " + threeDFormat.Perspective);

            // Yeni perspektif değerini ayarla (0 ile 120 derece arasında)
            threeDFormat.Perspective = 45;
            Console.WriteLine("Perspective set to: " + threeDFormat.Perspective);

            // Perspektif değişimini daha iyi görselleştirmek için diğer 3D efektleri uygula
            threeDFormat.ExtrusionHeight = 15;
            threeDFormat.ContourWidth = 2;
            threeDFormat.RotationX = 20;
            threeDFormat.RotationY = 30;

            // Etkileri görmek için çalışma kitabını kaydedin
            workbook.Save("ThreeDFormatPerspectiveDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


