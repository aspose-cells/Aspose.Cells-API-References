---
title: "FillFormat.GradientColorType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad FillFormat. Devuelve el tipo de color de degradado para el relleno especificado"
type: docs
url: /es/net/aspose.cells.drawing/fillformat/gradientcolortype/
---
## FillFormat.GradientColorType property

Devuelve el tipo de color de degradado para el relleno especificado.

```csharp
public GradientColorType GradientColorType { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class FillFormatPropertyGradientColorTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma para demostrar el relleno de degradado
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 1, 100, 200);

            try
            {
                // Establecer un relleno de degradado de dos colores
                shape.Fill.SetTwoColorGradient(Color.Red, Color.Blue,
                    GradientStyleType.Horizontal, 2);

                // Acceder a FillFormat para obtener GradientColorType
                FillFormat fillFormat = shape.Fill;

                // Mostrar el valor de GradientColorType
                Console.WriteLine("GradientColorType: " + fillFormat.GradientColorType);

                // Guarda el libro de trabajo
                workbook.Save("GradientColorTypeDemo.xlsx");
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

* enum [GradientColorType](../../gradientcolortype/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


