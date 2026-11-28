---
title: "Shape.Height"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Shape özelliği. Şeklin yüksekliğini piksel biriminde temsil eder"
type: docs
url: /tr/net/aspose.cells.drawing/shape/height/
---
## Shape.Height property

Şeklin yüksekliğini, piksel biriminde temsil eder.

```csharp
public int Height { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyHeightDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Gerekli tüm parametrelerle bir dikdörtgen şekil ekle
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 100);

            // İlk yüksekliği ayarla
            shape.Height = 150;
            Console.WriteLine("Initial height: " + shape.Height);

            // Yüksekliği koşullu olarak değiştir
            if (shape.Height == 150)
            {
                shape.Height = 100;
                Console.WriteLine("Modified height: " + shape.Height);
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


