---
title: "Shape.UpperDeltaY"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Shape özelliği. Şeklin üst sol köşe satırından dikey offsetini alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing/shape/upperdeltay/
---
## Shape.UpperDeltaY property

Şeklin sol üst köşe satırından dikey offsetini alır veya ayarlar.

```csharp
public int UpperDeltaY { get; set; }
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
    public class ShapePropertyUpperDeltaYDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // UpperDeltaY özelliğini göstermek için bir şekil ekle
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 100, 100);

            // İlk UpperDeltaY değerini ayarla ve göster
            shape.UpperDeltaY = 3;
            Console.WriteLine("Initial UpperDeltaY: " + shape.UpperDeltaY);

            // UpperDeltaY değerini değiştir
            if (shape.UpperDeltaY == 3)
            {
                shape.UpperDeltaY = 1;
                Console.WriteLine("Modified UpperDeltaY: " + shape.UpperDeltaY);
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


