---
title: "GradientFill.Angle"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad GradientFill. El ángulo del relleno lineal"
type: docs
url: /es/net/aspose.cells.drawing/gradientfill/angle/
---
## GradientFill.Angle property

El ángulo del relleno lineal.

```csharp
public float Angle { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class GradientFillPropertyAngleDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma para demostrar el relleno de degradado
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 200, 100);

            // Establecer propiedades del relleno de degradado
            shape.Fill.FillType = FillType.Gradient;
            shape.Fill.GradientFill.SetGradient(GradientFillType.Linear, 45, GradientDirectionType.FromCenter);
            shape.Fill.GradientFill.Angle = 45; // Set the angle to 45 degrees

            // Establecer colores del degradado
            shape.Fill.GradientFill.SetTwoColorGradient(
                Color.Red, 
                Color.Blue, 
                GradientStyleType.Horizontal, 
                1);

            // Guarda el libro de trabajo
            workbook.Save("GradientFillAngleDemo.xlsx");

            Console.WriteLine("Demo completed. File saved with gradient fill at 45 degree angle.");
        }
    }
}
```

### Ver también

* class [GradientFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


