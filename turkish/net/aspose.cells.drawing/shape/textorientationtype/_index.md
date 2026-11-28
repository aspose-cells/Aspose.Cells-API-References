---
title: "Shape.TextOrientationType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Shape özelliği. Şeklin metin yönlendirme tipini alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing/shape/textorientationtype/
---
## Shape.TextOrientationType property

Şeklin metin yönlendirme türünü alır ve ayarlar.

```csharp
public TextOrientationType TextOrientationType { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyTextOrientationTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına bir şekil ekle
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 200);

            // Şekil için metin ayarlayın
            shape.Text = "Sample Text";

            // Metin yönlendirmesini kontrol edin ve değiştirin
            if (shape.TextOrientationType == TextOrientationType.NoRotation)
            {
                shape.TextOrientationType = TextOrientationType.TopToBottom;
            }

            // Çalışma kitabını kaydedin
            workbook.Save("ShapeTextOrientationDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [TextOrientationType](../../../aspose.cells/textorientationtype/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


