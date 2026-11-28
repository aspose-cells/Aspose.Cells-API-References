---
title: "Shape.RotationAngle"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Shape özelliği. Şeklin dönüşünü alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing/shape/rotationangle/
---
## Shape.RotationAngle property

Şeklin dönüşünü alır ve ayarlar.

```csharp
public double RotationAngle { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyRotationAngleDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Gerekli tüm parametrelerle bir dikdörtgen şekil ekle
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 100, 200, 0, 0);

            // Dönme açısını 60 dereceye ayarla
            shape.RotationAngle = 60;
            Console.WriteLine("Shape rotation angle set to: " + shape.RotationAngle);

            // Mevcut dönme açısını al
            double currentAngle = shape.RotationAngle;
            Console.WriteLine("Current shape rotation angle: " + currentAngle);

            // Çalışma kitabını kaydedin
            workbook.Save("ShapeRotationDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


