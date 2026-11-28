---
title: "ShapeTextAlignment.RotationAngle"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ShapeTextAlignment özelliği. Şeklin dönüşünü alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing.texts/shapetextalignment/rotationangle/
---
## ShapeTextAlignment.RotationAngle property

Şeklin dönüşünü alır ve ayarlar.

```csharp
public double RotationAngle { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class ShapeTextAlignmentPropertyRotationAngleDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir dikdörtgen şekli ekle
            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 200, 300, 400);
            
            // Şekil metnini ayarla
            shape.Text = "Rotated Text";
            
            // Metin hizalamasına erişin ve dönüş açısını ayarlayın
            shape.TextBody.TextAlignment.RotationAngle = 90;

            // Çalışma kitabını kaydedin
            workbook.Save("ShapeTextRotationDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ShapeTextAlignment](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


