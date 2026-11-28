---
title: "Shape.UpperDeltaX"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Shape özelliği. Şeklin sol üst köşe sütunundan yatay ofsetini alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing/shape/upperdeltax/
---
## Shape.UpperDeltaX property

Şeklin sol üst köşe sütunundan yatay offsetini alır veya ayarlar.

```csharp
public int UpperDeltaX { get; set; }
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
    public class ShapePropertyUpperDeltaXDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına bir şekil ekle
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 0);

            // UpperDeltaX özelliğini ayarlayın ve görüntüleyin
            shape.UpperDeltaX = 150;
            Console.WriteLine("UpperDeltaX: " + shape.UpperDeltaX);

            // Koşulu karşıladığında UpperDeltaX'i değiştirin
            if (shape.UpperDeltaX == 150)
            {
                shape.UpperDeltaX = 100;
                Console.WriteLine("Modified UpperDeltaX: " + shape.UpperDeltaX);
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


