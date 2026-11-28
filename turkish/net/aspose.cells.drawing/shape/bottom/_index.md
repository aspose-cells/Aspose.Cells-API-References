---
title: "Shape.Bottom"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Shape özelliği. Şeklin alt köşe satırından dikey ofsetinin genişliğini piksel biriminde temsil eder"
type: docs
url: /tr/net/aspose.cells.drawing/shape/bottom/
---
## Shape.Bottom property

Şeklin alt köşe satırından dikey ofsetinin genişliğini, piksel biriminde temsil eder.

```csharp
public int Bottom { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyBottomDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Gerekli tüm parametrelerle bir örnek şekil ekle
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 100, 100);

            // İlk konumu ayarla
            shape.Top = 200;
            shape.Left = 200;

            // Bottom özelliğini göster
            Console.WriteLine("Original Bottom position: " + shape.Bottom);

            // Bottom konumunu değiştir
            if (shape.Bottom == 300)  // 200 (Top) + 100 (Height)
            {
                shape.Bottom = 250;  // This will change the Top position (250 - 100 = 150)
                Console.WriteLine("New Bottom position: " + shape.Bottom);
                Console.WriteLine("New Top position: " + shape.Top);
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


