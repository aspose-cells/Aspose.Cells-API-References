---
title: "Shape.LowerDeltaY"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Shape özelliği. Şeklin sağ alt köşe satırından dikey kaymasını alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing/shape/lowerdeltay/
---
## Shape.LowerDeltaY property

Şeklin alt sağ köşe satırından dikey ofsetini alır veya ayarlar.

```csharp
public int LowerDeltaY { get; set; }
```

### Açıklamalar

Değer aralığı 0 ile 256 arasındadır.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyLowerDeltaYDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Doğru parametrelerle örnek bir şekil ekleyin
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 100, 100);

            // LowerDeltaY özelliğini ayarlayın ve gösterin
            shape.LowerDeltaY = 20;
            Console.WriteLine("Initial LowerDeltaY: " + shape.LowerDeltaY);

            // LowerDeltaY'yi koşullu olarak değiştirin
            if (shape.LowerDeltaY == 20)
            {
                shape.LowerDeltaY = 10;
                Console.WriteLine("Modified LowerDeltaY: " + shape.LowerDeltaY);
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


