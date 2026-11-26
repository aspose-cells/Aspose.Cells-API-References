---
title: "Shape.TopCM"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Shape. Representa el desplazamiento vertical de la forma desde su fila superior en unidades de centímetros"
type: docs
url: /es/net/aspose.cells.drawing/shape/topcm/
---
## Shape.TopCM property

Representa el desplazamiento vertical de la forma desde su fila superior, en unidades de centímetros.

```csharp
public double TopCM { get; set; }
```

### Ejemplos

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

### Ver también

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


