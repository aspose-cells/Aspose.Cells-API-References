---
title: "Shape.TopCM"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Shape. Rappresenta lo spostamento verticale della forma dalla sua riga superiore in unità di centimetri"
type: docs
url: /it/net/aspose.cells.drawing/shape/topcm/
---
## Shape.TopCM property

Rappresenta lo spostamento verticale della forma dalla sua riga superiore, in centimetri.

```csharp
public double TopCM { get; set; }
```

### Esempi

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

### Vedi anche

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


