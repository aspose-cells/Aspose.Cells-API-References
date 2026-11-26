---
title: "Shape.GetConnectionPoints"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Shape. Obtiene los puntos de conexión"
type: docs
url: /es/net/aspose.cells.drawing/shape/getconnectionpoints/
---
## Shape.GetConnectionPoints method

Obtén los puntos de conexión

```csharp
public float[][] GetConnectionPoints()
```

### Valor de retorno

[X,Y] pairs of the connection point. Every item is a float[2] array, [0] represents x and [1] represents y.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodGetConnectionPointsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agrega una forma a la hoja de cálculo con todos los parámetros requeridos
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 0);

            // Obtener los puntos de conexión de la forma
            float[][] points = shape.GetConnectionPoints();

            // Mostrar los puntos de conexión
            Console.WriteLine("Connection Points:");
            for (int i = 0; i < points.Length; i++)
            {
                Console.WriteLine($"Point {i + 1}: X={points[i][0]}, Y={points[i][1]}");
            }
        }
    }
}
```

### Ver también

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


