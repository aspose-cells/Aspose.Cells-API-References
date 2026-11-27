---
title: "ReflectionEffect.Size"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ReflectionEffect property. Hämtar och anger slutpositionen längs alfa‑gradientens rampe för slut‑alfa‑värdet i procentenhet"
type: docs
url: /sv/net/aspose.cells.drawing/reflectioneffect/size/
---
## ReflectionEffect.Size property

Hämtar och anger slutpositionen (längs alfa gradientrampen) för slut-alfa-värdet, i enhet procent.

```csharp
public double Size { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ReflectionEffectPropertySizeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en shape
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 100);

            // Ställ in reflektionsegenskaper inklusive Storlek
            ReflectionEffect reflection = shape.Reflection;
            reflection.Type = ReflectionEffectType.HalfReflection4PtOffset;
            reflection.Transparency = 0.5;
            reflection.Size = 55.5;
            reflection.Blur = 0.5;
            reflection.Distance = 4;

            // Spara arbetsboken
            workbook.Save("output.xlsx");

            // Verifiera de sparade reflektionsegenskaperna
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            Shape loadedShape = loadedWorkbook.Worksheets[0].Shapes[0];
            ReflectionEffect loadedReflection = loadedShape.Reflection;

            Console.WriteLine("Reflection Size: " + loadedReflection.Size);
        }
    }
}
```

### Se även

* class [ReflectionEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


