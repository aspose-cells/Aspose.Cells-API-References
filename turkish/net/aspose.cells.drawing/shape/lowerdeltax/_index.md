---
title: "Shape.LowerDeltaX"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Shape özelliği. Şeklin alt sağ köşe sütunundan yatay ofsetini alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing/shape/lowerdeltax/
---
## Shape.LowerDeltaX property

Şeklin alt sağ köşe sütunundan yatay ofsetini alır veya ayarlar.

```csharp
public int LowerDeltaX { get; set; }
```

### Açıklamalar

Değer aralığı 0 ile 1024 arasındadır.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyLowerDeltaXDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir dikdörtgen şekli ekle
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 100, 100);

            // LowerDeltaX özelliğini ayarlayın ve gösterin
            shape.LowerDeltaX = 3;
            Console.WriteLine("Initial LowerDeltaX: " + shape.LowerDeltaX);

            // Koşul karşılandığında LowerDeltaX'i değiştirin
            if (shape.LowerDeltaX == 3)
            {
                shape.LowerDeltaX = 1;
                Console.WriteLine("Modified LowerDeltaX: " + shape.LowerDeltaX);
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


