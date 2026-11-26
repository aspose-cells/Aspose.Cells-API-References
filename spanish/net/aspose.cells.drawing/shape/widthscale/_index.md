---
title: "Shape.WidthScale"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Shape. Obtiene y establece la escala de ancho en unidades de porcentaje del ancho original de la imagen. Si la forma no es una imagen, la propiedad WidthScale solo devuelve 100"
type: docs
url: /es/net/aspose.cells.drawing/shape/widthscale/
---
## Shape.WidthScale property

Obtiene y establece la escala de ancho, en unidades de porcentaje del ancho original de la imagen. Si la forma no es una imagen, la propiedad WidthScale solo devuelve 100;

```csharp
public int WidthScale { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyWidthScaleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un shape rectangular con los parámetros correctos
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 0);

            // Establecer la escala de ancho inicial
            shape.WidthScale = 50;
            Console.WriteLine("Initial WidthScale: " + shape.WidthScale);

            // Modificar la escala de ancho si se cumple la condición
            if (shape.WidthScale == 50)
            {
                shape.WidthScale = 75;
                Console.WriteLine("Updated WidthScale: " + shape.WidthScale);
            }

            // Guarda el libro de trabajo
            workbook.Save("ShapeWidthScaleDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


