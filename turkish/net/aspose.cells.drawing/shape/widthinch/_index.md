---
title: "Shape.WidthInch"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Shape özelliği. Şeklin genişliğini inç biriminde temsil eder"
type: docs
url: /tr/net/aspose.cells.drawing/shape/widthinch/
---
## Shape.WidthInch property

Şeklin genişliğini inç biriminde temsil eder.

```csharp
public double WidthInch { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyWidthInchDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Gerekli tüm parametrelerle bir dikdörtgen şekil ekle
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 100);

            // Genişliği inç cinsinden ayarlayın
            shape.WidthInch = 3;
            Console.WriteLine("Shape width (inches): " + shape.WidthInch);

            // Koşul sağlandığında genişliği değiştirin
            if (shape.WidthInch == 3)
            {
                shape.WidthInch = 1;
                Console.WriteLine("Modified shape width (inches): " + shape.WidthInch);
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


