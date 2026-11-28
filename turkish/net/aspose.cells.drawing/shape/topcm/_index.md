---
title: "Shape.TopCM"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Shape özelliği. Şeklin üst satırından santimetre birimi cinsinden dikey offsetini temsil eder"
type: docs
url: /tr/net/aspose.cells.drawing/shape/topcm/
---
## Shape.TopCM property

Şeklin üst satırından dikey ofsetini santimetre biriminde temsil eder.

```csharp
public double TopCM { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyTopCMDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 100, 100);
            shape.TopCM = 3.0;
            
            Console.WriteLine("Shape Top position (cm): " + shape.TopCM);
            
            if (shape.TopCM == 3.0)
                shape.TopCM = 1.0;
                
            Console.WriteLine("Shape Top position after change (cm): " + shape.TopCM);
        }
    }
}
```

### Ayrıca Bakınız

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


