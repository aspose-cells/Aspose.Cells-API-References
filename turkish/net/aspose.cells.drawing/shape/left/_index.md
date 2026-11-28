---
title: "Shape.Left"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Shape özelliği. Şeklin sol sütundan yatay ofsetini piksel biriminde temsil eder"
type: docs
url: /tr/net/aspose.cells.drawing/shape/left/
---
## Shape.Left property

Şeklin sol sütunundan yatay ofsetini piksel biriminde temsil eder.

```csharp
public int Left { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyLeftDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Left özelliğini göstermek için bir şekil ekleyin
            Shape shape = worksheet.Shapes.AddRectangle(10, 10, 100, 100, 0, 0);

            // İlk Left konumunu ayarlayın
            shape.Left = 200;
            Console.WriteLine("Shape Left position: " + shape.Left);

            // Koşullu olarak Left konumunu değiştirin
            if (shape.Left == 200)
            {
                shape.Left = 150;
                Console.WriteLine("Adjusted Shape Left position: " + shape.Left);
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


