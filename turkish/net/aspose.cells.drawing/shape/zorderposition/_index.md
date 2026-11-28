---
title: "Shape.ZOrderPosition"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Shape özelliği. Bir şeklin z‑order içindeki konumunu döndürür"
type: docs
url: /tr/net/aspose.cells.drawing/shape/zorderposition/
---
## Shape.ZOrderPosition property

Bir şeklin z-sırasındaki konumunu döndürür.

```csharp
public int ZOrderPosition { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyZOrderPositionDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // ZOrder'ı göstermek için üç şekil ekle
            Shape shape1 = worksheet.Shapes.AddRectangle(10, 10, 100, 100, 0, 0);
            Shape shape2 = worksheet.Shapes.AddRectangle(50, 50, 100, 100, 0, 0);
            Shape shape3 = worksheet.Shapes.AddRectangle(90, 90, 100, 100, 0, 0);

            // ZOrder konumlarını ayarla
            shape1.ZOrderPosition = 0;
            shape2.ZOrderPosition = 1;
            shape3.ZOrderPosition = 2;

            // shape3'ün ZOrder'ını değiştirerek öne getir
            shape3.ZOrderPosition = 0;

            // Çalışma kitabını kaydedin
            workbook.Save("ShapeZOrderDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


