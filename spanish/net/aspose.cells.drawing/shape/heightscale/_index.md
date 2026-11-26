---
title: "Shape.HeightScale"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Shape. Obtiene y establece la escala de altura en unidades de porcentaje de la altura original de la imagen. Si la forma no es una imagen, la propiedad HeightScale solo devuelve 100"
type: docs
url: /es/net/aspose.cells.drawing/shape/heightscale/
---
## Shape.HeightScale property

Obtiene y establece la escala de altura, en porcentaje de la altura original de la imagen. Si la forma no es una imagen, la propiedad HeightScale solo devuelve 100;

```csharp
public int HeightScale { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyHeightScaleDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma rectangular
            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 200, 150);

            // Establecer la escala de altura inicial
            shape.HeightScale = 50;
            Console.WriteLine("Initial HeightScale: " + shape.HeightScale);

            // Modificar la escala de altura si se cumple la condición
            if (shape.HeightScale == 50)
            {
                shape.HeightScale = 75;
                Console.WriteLine("Modified HeightScale: " + shape.HeightScale);
            }
        }
    }
}
```

### Ver también

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


