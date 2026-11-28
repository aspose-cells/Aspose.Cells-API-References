---
title: "Shape.AutoShapeType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Shape özelliği. Otomatik şekil tipini alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing/shape/autoshapetype/
---
## Shape.AutoShapeType property

Otomatik şekil tipini alır ve ayarlar.

```csharp
public AutoShapeType AutoShapeType { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyAutoShapeTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına doğru parametrelerle bir şekil ekleyin
            Shape shape = worksheet.Shapes.AddAutoShape(AutoShapeType.Rectangle, 1, 1, 100, 150, 0, 0);

            // Gerekirse AutoShapeType'ı kontrol edin ve değiştirin
            if (shape.AutoShapeType == AutoShapeType.Unknown)
            {
                shape.AutoShapeType = AutoShapeType.Rectangle;
            }

            // Özelliği göstermek için şekil tipini değiştirin
            shape.AutoShapeType = AutoShapeType.Oval;

            // Çalışma kitabını kaydedin
            workbook.Save("ShapePropertyAutoShapeTypeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [AutoShapeType](../../autoshapetype/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


