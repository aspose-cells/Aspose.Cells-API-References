---
title: "Shape.ThreeDFormat"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Shape özelliği. Şeklin 3D formatını alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing/shape/threedformat/
---
## Shape.ThreeDFormat property

Şeklin 3D biçimini alır ve ayarlar.

```csharp
public ThreeDFormat ThreeDFormat { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyThreeDFormatDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Gerekli tüm parametrelerle bir örnek şekil ekle
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 100);

            // 3D format özelliklerine eriş ve değiştir
            ThreeDFormat threeDFormat = shape.ThreeDFormat;
            threeDFormat.ExtrusionColor.Color = System.Drawing.Color.Blue;
            threeDFormat.LightAngle = 45;
            threeDFormat.ContourWidth = 2;
            threeDFormat.ContourColor.Color = System.Drawing.Color.Red;

            // Çalışma kitabını kaydedin
            workbook.Save("ThreeDFormatDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ThreeDFormat](../../threedformat/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


