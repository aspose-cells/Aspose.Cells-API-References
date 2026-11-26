---
title: "Class ShadowEffect"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.Drawing.ShadowEffect class. Esta clase especifica el efecto de sombra del elemento del gráfico o forma"
type: docs
url: /es/net/aspose.cells.drawing/shadoweffect/
---
## ShadowEffect class

Esta clase especifica el efecto de sombra del elemento del gráfico o forma.

```csharp
public class ShadowEffect
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Angle](../../aspose.cells.drawing/shadoweffect/angle/) { get; set; } | Obtiene y establece el ángulo de iluminación. Rango de 0 a 359,9 grados. |
| [Blur](../../aspose.cells.drawing/shadoweffect/blur/) { get; set; } | Obtiene y establece el desenfoque de la sombra. Rango de 0 a 100 puntos. |
| [Color](../../aspose.cells.drawing/shadoweffect/color/) { get; set; } | Obtiene y establece el color de la sombra. |
| [Distance](../../aspose.cells.drawing/shadoweffect/distance/) { get; set; } | Obtiene y establece la distancia de la sombra. Rango de 0 a 200 puntos. |
| [PresetType](../../aspose.cells.drawing/shadoweffect/presettype/) { get; set; } | Obtiene y establece el tipo de sombra predefinido de la sombra. |
| [Size](../../aspose.cells.drawing/shadoweffect/size/) { get; set; } | Obtiene y establece el tamaño de la sombra. Rango de 0 a 2.0. No tiene sentido en sombra interna. |
| [Transparency](../../aspose.cells.drawing/shadoweffect/transparency/) { get; set; } | Obtiene y establece el grado de transparencia de la sombra. Rango de 0.0 (opaco) a 1.0 (claro). |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassShadowEffectDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma de ejemplo con todos los parámetros requeridos
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 100);

            // Obtener el efecto de sombra de la forma
            ShadowEffect shadow = shape.ShadowEffect;

            // Establecer propiedades de la sombra
            shadow.Angle = 150;
            shadow.Blur = 30;
            shadow.Size = 1.3;
            shadow.Transparency = 0.4;
            shadow.Distance = 80;

            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");

            Console.WriteLine("Shadow effect demo completed successfully.");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


