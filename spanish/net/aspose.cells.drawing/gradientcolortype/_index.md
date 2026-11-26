---
title: "Enum GradientColorType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enum Aspose.Cells.Drawing.GradientColorType. Representa el tipo de color de degradado para el relleno especificado"
type: docs
url: /es/net/aspose.cells.drawing/gradientcolortype/
---
## GradientColorType enumeration

Representa el tipo de color degradado para el relleno especificado.

```csharp
public enum GradientColorType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| None | `0` | Sin color de degradado |
| OneColor | `1` | Un color de degradado |
| PresetColors | `2` | Colores de degradado predefinidos |
| TwoColors | `3` | Dos colores de degradado |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class DrawingClassGradientColorTypeDemo
    {
        public static void Run()
        {
            // Cree un nuevo libro de trabajo para la demostración
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Agregar una forma para demostrar el relleno de degradado
                Shape shape = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 200, 200);
                FillFormat fill = shape.Fill;

                // Establecer el tipo de relleno de degradado
                fill.FillType = FillType.Gradient;

                // Demostrar los diferentes valores del enum GradientColorType
                Console.WriteLine("Available GradientColorType values:");
                Console.WriteLine("None: " + GradientColorType.None);
                Console.WriteLine("OneColor: " + GradientColorType.OneColor);
                Console.WriteLine("PresetColors: " + GradientColorType.PresetColors);
                Console.WriteLine("TwoColors: " + GradientColorType.TwoColors);

                // Leer y mostrar el tipo de color de degradado actual (la propiedad es de solo lectura)
                Console.WriteLine("Current gradient color type: " + fill.GradientColorType);

                // Guarda el libro de trabajo
                workbook.Save("GradientColorTypeDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with GradientColorType: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


