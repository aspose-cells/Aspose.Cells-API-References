---
title: "Shape.HeightPt"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Shape özelliği. Şeklin yüksekliğini puan biriminde temsil eder"
type: docs
url: /tr/net/aspose.cells.drawing/shape/heightpt/
---
## Shape.HeightPt property

Şeklin yüksekliğini puan biriminde temsil eder.

```csharp
public double HeightPt { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyHeightPtDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Gerekli tüm parametrelerle bir örnek şekil ekle
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 50, 100);

            // HeightPt özelliğini ayarlayın ve alın
            shape.HeightPt = 50;
            Console.WriteLine("Shape height in points: " + shape.HeightPt);

            // Koşulu karşılıyorsa yüksekliği değiştirin
            if (shape.HeightPt == 50)
            {
                shape.HeightPt = 30;
                Console.WriteLine("Modified shape height: " + shape.HeightPt);
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


