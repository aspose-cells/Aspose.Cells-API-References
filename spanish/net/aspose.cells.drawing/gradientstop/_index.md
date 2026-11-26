---
title: "Clase GradientStop"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Drawing.GradientStop. Representa la parada de degradado"
type: docs
url: /es/net/aspose.cells.drawing/gradientstop/
---
## GradientStop class

Representa la parada de degradado.

```csharp
public class GradientStop
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [CellsColor](../../aspose.cells.drawing/gradientstop/cellscolor/) { get; } | Obtiene el color de esta parada de degradado. |
| [Position](../../aspose.cells.drawing/gradientstop/position/) { get; set; } | La posición de la parada. |
| [Transparency](../../aspose.cells.drawing/gradientstop/transparency/) { get; set; } | Devuelve o establece el grado de transparencia del área como un valor de 0.0 (opaco) a 1.0 (claro). |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class DrawingClassGradientStopDemo
    {
        public static void Run()
        {
            // Cree un nuevo libro de trabajo para la demostración
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Agregar una forma con relleno degradado
                Shape shape = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 100, 300);
                shape.Fill.FillType = FillType.Gradient;
                GradientFill gradientFill = shape.Fill.GradientFill;
                gradientFill.SetGradient(GradientFillType.Linear, 0, GradientDirectionType.FromUpperLeftCorner);

                // Crear color para la parada de degradado
                CellsColor color = workbook.CreateCellsColor();
                color.Color = Color.Blue;

                // Agregar parada de degradado
                gradientFill.GradientStops.Add(0, color, 30);

                // Acceder a la parada de degradado
                GradientStop stop = gradientFill.GradientStops[0];

                // Demuestra la funcionalidad básica
                Console.WriteLine("GradientStop instance created successfully");
                Console.WriteLine("Position: " + stop.Position);
                Console.WriteLine("Transparency: " + stop.Transparency);
                Console.WriteLine("CellsColor Type: " + stop.CellsColor.Type);

                // Modificar propiedades
                stop.Position = 0.5;
                stop.Transparency = 0.7;

                Console.WriteLine("Modified Position: " + stop.Position);
                Console.WriteLine("Modified Transparency: " + stop.Transparency);

                // Guarda el libro de trabajo
                workbook.Save("GradientStopDemo.xlsx");
                Console.WriteLine("Demo completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with GradientStop: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


