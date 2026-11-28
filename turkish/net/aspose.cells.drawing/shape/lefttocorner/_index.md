---
title: "Shape.LeftToCorner"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Shape özelliği. Şeklin çalışma sayfasının sol kenarından yatay ofsetini alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing/shape/lefttocorner/
---
## Shape.LeftToCorner property

Şeklin çalışma sayfasının sol kenarından yatay ofsetini alır ve ayarlar.

```csharp
public int LeftToCorner { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyLeftToCornerDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Doğru parametrelerle bir dikdörtgen şekil ekle
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 150, 0);

            // LeftToCorner özelliğini ayarlayın ve gösterin
            shape.LeftToCorner = 50;
            Console.WriteLine("Shape LeftToCorner value: " + shape.LeftToCorner);

            // LeftToCorner'ı belirli bir değere eşitse değiştirin
            if (shape.LeftToCorner == 50)
            {
                shape.LeftToCorner = 30;
                Console.WriteLine("Modified LeftToCorner value: " + shape.LeftToCorner);
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


