---
title: "Shape.Top"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Shape. Representa el desplazamiento vertical de la forma desde su fila superior en unidades de píxeles"
type: docs
url: /es/net/aspose.cells.drawing/shape/top/
---
## Shape.Top property

Representa el desplazamiento vertical de la forma desde su fila superior, en unidades de píxeles.

```csharp
public int Top { get; set; }
```

### Observaciones

Si la forma está en el gráfico, representa el desplazamiento vertical de la forma desde su borde superior.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyTopDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma rectangular
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 100, 100);

            // Establecer la posición superior inicial
            shape.Top = 50;
            Console.WriteLine("Initial Top position: " + shape.Top);

            // Modificar la posición superior si es igual a 3 (demostrando la lógica del caso de prueba)
            if (shape.Top == 3)
            {
                shape.Top = 1;
            }
            else
            {
                // Para demostración, establecer en 3 y luego aplicar la lógica del caso de prueba
                shape.Top = 3;
                if (shape.Top == 3)
                {
                    shape.Top = 1;
                    Console.WriteLine("Modified Top position: " + shape.Top);
                }
            }
        }
    }
}
```

### Ver también

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


