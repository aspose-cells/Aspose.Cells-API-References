---
title: "Clase GradientFill"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Drawing.GradientFill. Representa el relleno degradado"
type: docs
url: /es/net/aspose.cells.drawing/gradientfill/
---
## GradientFill class

Representa el relleno degradado.

```csharp
public class GradientFill : Fill
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Angle](../../aspose.cells.drawing/gradientfill/angle/) { get; set; } | El ángulo del relleno lineal. |
| [DirectionType](../../aspose.cells.drawing/gradientfill/directiontype/) { get; } | Obtiene el tipo de dirección del degradado. |
| [FillType](../../aspose.cells.drawing/gradientfill/filltype/) { get; } | Obtiene el tipo de relleno degradado. |
| [GradientStops](../../aspose.cells.drawing/gradientfill/gradientstops/) { get; } | Representa la colección de paradas de degradado. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| override [Equals](../../aspose.cells.drawing/fill/equals/)(object) | /(Hereda de [`Fill`](../fill/).) |
| override [GetHashCode](../../aspose.cells.drawing/fill/gethashcode/)() | Obtiene el código hash.(Hereda de [`Fill`](../fill/).) |
| [SetGradient](../../aspose.cells.drawing/gradientfill/setgradient/)(GradientFillType, double, GradientDirectionType) | Establecer el tipo y la dirección del relleno degradado. |
| [SetOneColorGradient](../../aspose.cells.drawing/gradientfill/setonecolorgradient/)(Color, double, GradientStyleType, int) | Establece el relleno especificado a un degradado de un color. Solo se aplica a Excel 2007. |
| [SetPresetThemeGradient](../../aspose.cells.drawing/gradientfill/setpresetthemegradient/)(PresetThemeGradientType, ThemeColorType) | Establece el relleno degradado de tema preestablecido. |
| [SetTwoColorGradient](../../aspose.cells.drawing/gradientfill/settwocolorgradient/#settwocolorgradient_1)(Color, Color, GradientStyleType, int) | Establece el relleno especificado a un degradado de dos colores. Solo se aplica a Excel 2007. |
| [SetTwoColorGradient](../../aspose.cells.drawing/gradientfill/settwocolorgradient/#settwocolorgradient)(Color, double, Color, double, GradientStyleType, int) | Establece el relleno especificado a un degradado de dos colores. Solo se aplica a Excel 2007. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System.Drawing;

    public class DrawingClassGradientFillDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una shape rectangular a la worksheet con todos los parámetros requeridos
            Shape shape = worksheet.Shapes.AddRectangle(5, 5, 0, 0, 150, 100);

            // Establecer el tipo de relleno a degradado para acceder a las propiedades del relleno degradado
            shape.Fill.FillType = FillType.Gradient;

            // Obtener la instancia existente del relleno degradado de la shape
            GradientFill gradientFill = shape.Fill.GradientFill;

            // Configurar el degradado con dos colores usando la instancia existente
            gradientFill.SetTwoColorGradient(
                Color.LightSkyBlue,  // First color
                Color.DarkBlue,      // Second color
                GradientStyleType.Horizontal, // Gradient style
                1                    // Variant
            );

            // Guarda el libro de trabajo
            workbook.Save("GradientFillDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Fill](../fill/)
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


