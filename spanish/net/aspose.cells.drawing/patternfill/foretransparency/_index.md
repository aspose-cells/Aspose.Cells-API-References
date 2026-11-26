---
title: "PatternFill.ForeTransparency"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PatternFill. Obtiene o establece la transparencia del color de primer plano"
type: docs
url: /es/net/aspose.cells.drawing/patternfill/foretransparency/
---
## PatternFill.ForeTransparency property

Obtiene o establece la transparencia del color de primer plano.

```csharp
public double ForeTransparency { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class PatternFillPropertyForeTransparencyDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Añade una forma rectangular para demostrar el relleno de patrón
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 200, 100);

            // Establece el tipo de relleno a patrón
            shape.Fill.FillType = FillType.Pattern;

            // Obtén la instancia de PatternFill
            PatternFill patternFill = shape.Fill.PatternFill;

            // Configura las propiedades de relleno de patrón
            patternFill.Pattern = FillPattern.Solid;
            patternFill.ForegroundColor = Color.Red;
            patternFill.BackgroundColor = Color.Blue;

            try
            {
                // Muestra el valor inicial de ForeTransparency
                Console.WriteLine("Initial ForeTransparency value: " + patternFill.ForeTransparency);

                // Establece un nuevo valor de ForeTransparency (50% de transparencia)
                patternFill.ForeTransparency = 0.5;

                // Muestra el valor actualizado de ForeTransparency
                Console.WriteLine("Updated ForeTransparency value: " + patternFill.ForeTransparency);

                // Guarda el libro de trabajo
                workbook.Save("ForeTransparencyDemo.xlsx");
                Console.WriteLine("ForeTransparency demonstration completed successfully.");
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

* class [PatternFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


