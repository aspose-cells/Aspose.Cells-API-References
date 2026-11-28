---
title: "Shape.HeightCM"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Shape özelliği. Şeklin yüksekliğini santimetre biriminde temsil eder"
type: docs
url: /tr/net/aspose.cells.drawing/shape/heightcm/
---
## Shape.HeightCM property

Şeklin yüksekliğini santimetre biriminde temsil eder.

```csharp
public double HeightCM { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyHeightCMDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Gerekli tüm parametrelerle bir dikdörtgen şekil ekle
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 100, 100);

            // Yüksekliği santimetre cinsinden ayarlayın
            shape.HeightCM = 3;
            Console.WriteLine("Shape height: " + shape.HeightCM + " cm");

            // Yüksekliği 3 cm ise değiştirin
            if (shape.HeightCM == 3)
            {
                shape.HeightCM = 1;
                Console.WriteLine("Modified shape height: " + shape.HeightCM + " cm");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


