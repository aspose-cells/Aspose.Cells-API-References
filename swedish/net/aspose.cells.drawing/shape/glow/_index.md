---
title: "Shape.Glow"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Shape-egenskap. Representerar ett GlowEffect-objekt som specificerar glödeffekt för diagramelementet eller formen"
type: docs
url: /sv/net/aspose.cells.drawing/shape/glow/
---
## Shape.Glow property

Representerar ett [`GlowEffect`](../../gloweffect/)-objekt som specificerar glödeffekt för diagramelementet eller formen.

```csharp
public GlowEffect Glow { get; }
```

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en rektangelform
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 150);

            // Åtkomst till glödeffekten
            GlowEffect glow = shape.Glow;

            // Ange glödegenskaper
            CellsColor color = workbook.CreateCellsColor();
            color.Color = System.Drawing.Color.Purple;
            glow.Color = color;
            glow.Size = 10; // 10 point radius
            glow.Transparency = 0.5; // 50% transparency

            // Spara arbetsboken
            workbook.Save("ShapeGlowDemo.xlsx");
        }
    }
}
```

### Se även

* class [GlowEffect](../../gloweffect/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


