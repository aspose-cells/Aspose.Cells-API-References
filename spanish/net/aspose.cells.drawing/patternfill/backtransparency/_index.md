---
title: "PatternFill.BackTransparency"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PatternFill. Obtiene o establece la transparencia del color de fondo"
type: docs
url: /es/net/aspose.cells.drawing/patternfill/backtransparency/
---
## PatternFill.BackTransparency property

Obtiene o establece la transparencia del color de fondo.

```csharp
public double BackTransparency { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class PatternFillPropertyBackTransparencyDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agrega una forma rectangular a la hoja de cálculo
            Shape shape = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 200, 200);

            // Obtén la instancia existente de PatternFill del shape y configura sus propiedades
            shape.Fill.FillType = FillType.Pattern;
            PatternFill patternFill = shape.Fill.PatternFill;
            patternFill.Pattern = FillPattern.Solid;
            patternFill.BackgroundColor = Color.Blue;

            // Muestra el valor inicial de BackTransparency
            Console.WriteLine("Current BackTransparency value: " + patternFill.BackTransparency);

            // Establece un nuevo valor de BackTransparency (50% de transparencia)
            patternFill.BackTransparency = 0.5;

            // Guardar el libro de trabajo modificado
            workbook.Save("PatternFillBackTransparencyDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PatternFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


