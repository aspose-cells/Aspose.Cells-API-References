---
title: "Clase GlowEffect"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Drawing.GlowEffect. Esta clase especifica un efecto de resplandor en el que se agrega un contorno difuso de color fuera de los bordes del objeto"
type: docs
url: /es/net/aspose.cells.drawing/gloweffect/
---
## GlowEffect class

Esta clase especifica un efecto de resplandor, en el que se añade un contorno difuminado de color fuera de los bordes del objeto.

```csharp
public class GlowEffect
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Color](../../aspose.cells.drawing/gloweffect/color/) { get; set; } | Obtiene el color del efecto de resplandor. |
| [Radius](../../aspose.cells.drawing/gloweffect/radius/) { get; set; } | (**Obsoleto.**) Obtiene y establece el radio del resplandor, en unidades de puntos. |
| [Size](../../aspose.cells.drawing/gloweffect/size/) { get; set; } | Obtiene y establece el radio del resplandor, en unidades de puntos. |
| [Transparency](../../aspose.cells.drawing/gloweffect/transparency/) { get; set; } | Obtiene y establece el grado de transparencia del efecto de resplandor. Rango de 0.0 (opaco) a 1.0 (claro). |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class GlowEffectDemo
    {
        public static void GlowEffectExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma de arco a la hoja de cálculo
            ArcShape arcShape = worksheet.Shapes.AddArc(2, 0, 2, 0, 130, 130);

            // Establecer la posición del arco
            arcShape.Placement = PlacementType.FreeFloating;

            // Establecer el formato de relleno
            arcShape.Fill.FillType = FillType.Solid;
            arcShape.Fill.SolidFill.Color = Color.Blue;

            // Establecer el estilo de línea
            arcShape.Line.CompoundType = MsoLineStyle.Single;
            arcShape.Line.Weight = 2;
            arcShape.Line.FillType = FillType.Solid;
            arcShape.Line.SolidFill.Color = Color.Red;
            arcShape.Line.DashStyle = MsoLineDashStyle.Solid;

            // Crear una instancia de GlowEffect y establecer sus propiedades
            GlowEffect glowEffect = arcShape.Glow;
            glowEffect.Color = workbook.CreateCellsColor();
            glowEffect.Color.Color = Color.Yellow;
            glowEffect.Radius = 10.0;
            glowEffect.Transparency = 0.5;

            // Guarda el libro de trabajo
            workbook.Save("GlowEffectExample.xlsx");
            workbook.Save("GlowEffectExample.pdf");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


