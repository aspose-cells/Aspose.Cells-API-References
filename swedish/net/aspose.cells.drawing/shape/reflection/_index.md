---
title: "Shape.Reflection"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Shape‑egenskap. Representerar ett ReflectionEffect‑objekt som specificerar reflektionseffekt för diagram‑elementet eller formen."
type: docs
url: /sv/net/aspose.cells.drawing/shape/reflection/
---
## Shape.Reflection property

Representerar ett [`ReflectionEffect`](../../reflectioneffect/)‑objekt som specificerar reflektionseffekt för diagram‑elementet eller formen.

```csharp
public ReflectionEffect Reflection { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyReflectionDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en rektangelform
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 150);

            // Ställ in reflektionsegenskaper
            ReflectionEffect reflection = shape.Reflection;
            reflection.Blur = 5;
            reflection.Distance = 10;
            reflection.Direction = 90;
            reflection.FadeDirection = 90;
            reflection.Size = 50;
            reflection.Transparency = 0.5;
            reflection.Type = ReflectionEffectType.None;

            // Spara arbetsboken
            workbook.Save("ShapeReflectionDemo.xlsx");
        }
    }
}
```

### Se även

* class [ReflectionEffect](../../reflectioneffect/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


