---
title: "Shape.Glow"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Shape. Representa un objeto GlowEffect que especifica el efecto de brillo para el elemento del gráfico o la forma"
type: docs
url: /es/net/aspose.cells.drawing/shape/glow/
---
## Shape.Glow property

Representa un objeto [`GlowEffect`](../../gloweffect/) que especifica el efecto de brillo para el elemento del gráfico o la forma.

```csharp
public GlowEffect Glow { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyGlowDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma rectangular
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 150);

            // Acceder al efecto de brillo
            GlowEffect glow = shape.Glow;

            // Establecer propiedades de brillo
            CellsColor color = workbook.CreateCellsColor();
            color.Color = System.Drawing.Color.Purple;
            glow.Color = color;
            glow.Size = 10; // 10 point radius
            glow.Transparency = 0.5; // 50% transparency

            // Guarda el libro de trabajo
            workbook.Save("ShapeGlowDemo.xlsx");
        }
    }
}
```

### Ver también

* class [GlowEffect](../../gloweffect/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


