---
title: "Shape.TopCM"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Shape. Представляет вертикальное смещение фигуры от её верхней строки в сантиметрах"
type: docs
url: /ru/net/aspose.cells.drawing/shape/topcm/
---
## Shape.TopCM property

Представляет вертикальное смещение фигуры от её верхней строки в сантиметрах.

```csharp
public double TopCM { get; set; }
```

### Примеры

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

### См. также

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


