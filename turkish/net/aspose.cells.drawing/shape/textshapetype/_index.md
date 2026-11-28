---
title: "Shape.TextShapeType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Shape property. Önceden ayarlanmış metin şekli tipini alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing/shape/textshapetype/
---
## Shape.TextShapeType property

Önceden ayarlanmış metin şekli türünü alır ve ayarlar.

```csharp
public AutoShapeType TextShapeType { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyTextShapeTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Doğru parametrelerle bir dikdörtgen şekil ekle
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 150, 0);

            // Bilinmiyorsa TextShapeType'ı kontrol edin ve ayarlayın
            if (shape.TextShapeType == AutoShapeType.Unknown)
            {
                shape.TextShapeType = AutoShapeType.Rectangle;
            }

            // Şeklin TextShapeType'ını çıktılayın
            Console.WriteLine("Shape TextShapeType: " + shape.TextShapeType);
        }
    }
}
```

### Ayrıca Bakınız

* enum [AutoShapeType](../../autoshapetype/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


