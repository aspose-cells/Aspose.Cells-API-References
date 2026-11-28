---
title: "Shape.LeftInch"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Shape özelliği. Şeklin sol sütunundan inç biriminde yatay kaymasını temsil eder"
type: docs
url: /tr/net/aspose.cells.drawing/shape/leftinch/
---
## Shape.LeftInch property

Şeklin sol sütunundan yatay ofsetini inç biriminde temsil eder.

```csharp
public double LeftInch { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyLeftInchDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Gerekli tüm parametrelerle bir örnek şekil ekle
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 100, 100);

            // LeftInch özelliğini ayarlayın ve gösterin
            shape.LeftInch = 3;
            Console.WriteLine("Shape left position (inches): " + shape.LeftInch);

            // Sol konumu 3 inç ise değiştirin
            if (shape.LeftInch == 3)
            {
                shape.LeftInch = 1;
                Console.WriteLine("Adjusted shape left position (inches): " + shape.LeftInch);
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


