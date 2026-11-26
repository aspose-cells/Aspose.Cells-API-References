---
title: "GradientStop.CellsColor"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad GradientStop. Obtiene el color de este punto de degradado"
type: docs
url: /es/net/aspose.cells.drawing/gradientstop/cellscolor/
---
## GradientStop.CellsColor property

Obtiene el color de esta parada de degradado.

```csharp
public CellsColor CellsColor { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class GradientStopPropertyCellsColorDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
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

                // Acceder al punto de degradado y mostrar sus propiedades CellsColor
                GradientStop stop = gradientFill.GradientStops[0];
                CellsColor stopColor = stop.CellsColor;

                Console.WriteLine("Gradient Stop CellsColor Properties:");
                Console.WriteLine("Color Type: " + stopColor.Type);
                Console.WriteLine("RGB Color: " + stopColor.Color);
                Console.WriteLine("ARGB Value: " + stopColor.Argb);
                Console.WriteLine("Transparency: " + stopColor.Transparency);

                // Guarda el libro de trabajo
                workbook.Save("GradientStopCellsColorDemo.xlsx");
                Console.WriteLine("Demo completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [CellsColor](../../../aspose.cells/cellscolor/)
* class [GradientStop](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


