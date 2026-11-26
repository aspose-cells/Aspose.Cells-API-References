---
title: "ShadowEffect.Distance"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ShadowEffect. Obtiene y establece la distancia de la sombra. Rango de 0 a 200 puntos"
type: docs
url: /es/net/aspose.cells.drawing/shadoweffect/distance/
---
## ShadowEffect.Distance property

Obtiene y establece la distancia de la sombra. Rango de 0 a 200 puntos.

```csharp
public double Distance { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShadowEffectPropertyDistanceDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma rectangular
            RectangleShape rectangle = worksheet.Shapes.AddRectangle(2, 0, 2, 0, 150, 100);
            
            // Configurar el efecto de sombra
            ShadowEffect shadow = rectangle.ShadowEffect;
            shadow.PresetType = PresetShadowType.OffsetDiagonalTopRight;
            
            // Crear un objeto CellsColor y establecer valores ARGB
            CellsColor color = workbook.CreateCellsColor();
            color.Argb = (128 << 24) | (255 << 16) | (0 << 8) | 0; // Semi-transparent red
            shadow.Color = color;
            
            shadow.Transparency = 0.3;
            shadow.Blur = 15;
            shadow.Angle = 45;
            shadow.Distance = 20; // Set distance to 20 points

            // Mostrar la distancia de la sombra
            Console.WriteLine("Shadow Distance: " + shadow.Distance + " points");

            // Guardar el libro de trabajo con efecto de sombra
            workbook.Save("ShadowEffectPropertyDistanceDemo_out.xlsx");
        }
    }
}
```

### Ver también

* class [ShadowEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


