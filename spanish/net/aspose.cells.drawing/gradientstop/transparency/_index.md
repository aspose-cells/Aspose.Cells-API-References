---
title: "GradientStop.Transparency"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad GradientStop. Devuelve o establece el grado de transparencia del área como un valor de 0.0 opaco a 1.0 transparente"
type: docs
url: /es/net/aspose.cells.drawing/gradientstop/transparency/
---
## GradientStop.Transparency property

Devuelve o establece el grado de transparencia del área como un valor de 0.0 (opaco) a 1.0 (claro).

```csharp
public double Transparency { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class GradientStopPropertyTransparencyDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma con relleno degradado
            Shape shape = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 100, 300);
            shape.Fill.FillType = FillType.Gradient;
            GradientFill gradientFill = shape.Fill.GradientFill;
            gradientFill.SetGradient(GradientFillType.Linear, 0, GradientDirectionType.FromUpperLeftCorner);

            // Crear color para la parada de degradado
            CellsColor color = workbook.CreateCellsColor();
            color.Color = Color.Blue;

            // Agregar un punto de degradado con transparencia inicial
            gradientFill.GradientStops.Add(0, color, 30);

            // Acceder a la parada de degradado
            GradientStop stop = gradientFill.GradientStops[0];

            // Mostrar y modificar la transparencia
            Console.WriteLine("Initial Transparency: " + stop.Transparency);
            stop.Transparency = 0.7;
            Console.WriteLine("Modified Transparency: " + stop.Transparency);

            // Agregar otro punto para comparación visual
            CellsColor color2 = workbook.CreateCellsColor();
            color2.Color = Color.Green;
            gradientFill.GradientStops.Add(1, color2, 30);

            // Guarda el libro de trabajo
            workbook.Save("GradientStopTransparencyDemo.xlsx");
        }
    }
}
```

### Ver también

* class [GradientStop](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


