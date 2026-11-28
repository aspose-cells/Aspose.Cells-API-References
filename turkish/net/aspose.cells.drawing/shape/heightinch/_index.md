---
title: "Shape.HeightInch"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Shape özelliği. Şeklin yüksekliğini inç biriminde temsil eder"
type: docs
url: /tr/net/aspose.cells.drawing/shape/heightinch/
---
## Shape.HeightInch property

Şeklin yüksekliğini inç biriminde temsil eder.

```csharp
public double HeightInch { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyHeightInchDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Gerekli tüm parametrelerle bir dikdörtgen şekil ekle
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 100);

            // Yüksekliği inç cinsinden ayarlayın ve alın
            shape.HeightInch = 3;
            Console.WriteLine("Shape height (inches): " + shape.HeightInch);

            // Koşul sağlandığında yüksekliği değiştirin
            if (shape.HeightInch == 3)
            {
                shape.HeightInch = 1;
                Console.WriteLine("Modified shape height (inches): " + shape.HeightInch);
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


