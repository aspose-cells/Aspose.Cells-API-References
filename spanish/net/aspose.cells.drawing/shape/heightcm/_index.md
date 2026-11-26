---
title: "Shape.HeightCM"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Shape. Representa la altura de la forma en unidades de centímetros"
type: docs
url: /es/net/aspose.cells.drawing/shape/heightcm/
---
## Shape.HeightCM property

Representa la altura de la forma, en unidades de centímetros.

```csharp
public double HeightCM { get; set; }
```

### Ejemplos

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

            // Agregar una forma rectangular con todos los parámetros requeridos
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 100, 100);

            // Establecer la altura en centímetros
            shape.HeightCM = 3;
            Console.WriteLine("Shape height: " + shape.HeightCM + " cm");

            // Modificar la altura si es 3 cm
            if (shape.HeightCM == 3)
            {
                shape.HeightCM = 1;
                Console.WriteLine("Modified shape height: " + shape.HeightCM + " cm");
            }
        }
    }
}
```

### Ver también

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


