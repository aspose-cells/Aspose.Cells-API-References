---
title: "Shape.RotationAngle"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Shape. Obtiene y establece la rotación de la forma"
type: docs
url: /es/net/aspose.cells.drawing/shape/rotationangle/
---
## Shape.RotationAngle property

Obtiene y establece la rotación de la forma.

```csharp
public double RotationAngle { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyRotationAngleDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma rectangular con todos los parámetros requeridos
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 100, 200, 0, 0);

            // Establecer el ángulo de rotación a 60 grados
            shape.RotationAngle = 60;
            Console.WriteLine("Shape rotation angle set to: " + shape.RotationAngle);

            // Obtener el ángulo de rotación actual
            double currentAngle = shape.RotationAngle;
            Console.WriteLine("Current shape rotation angle: " + currentAngle);

            // Guarda el libro de trabajo
            workbook.Save("ShapeRotationDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


