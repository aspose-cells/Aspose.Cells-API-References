---
title: "Klass ReflectionEffect"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Drawing.ReflectionEffect klass. Denna klass specificerar en reflektionseffekt"
type: docs
url: /sv/net/aspose.cells.drawing/reflectioneffect/
---
## ReflectionEffect class

Denna klass specificerar en reflektseffekt.

```csharp
public class ReflectionEffect
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Blur](../../aspose.cells.drawing/reflectioneffect/blur/) { get; set; } | Hämtar och anger oskarphetsradien, i enheter av punkter. |
| [Direction](../../aspose.cells.drawing/reflectioneffect/direction/) { get; set; } | Hämtar och anger riktningen för alfa gradientrampen relativt formen själv. |
| [Distance](../../aspose.cells.drawing/reflectioneffect/distance/) { get; set; } | Hämtar och anger hur långt skuggan ska förskjutas, i enheter av punkter. |
| [FadeDirection](../../aspose.cells.drawing/reflectioneffect/fadedirection/) { get; set; } | Hämtar och anger riktningen för att förskjuta reflektionen. |
| [RotWithShape](../../aspose.cells.drawing/reflectioneffect/rotwithshape/) { get; set; } | Hämtar och anger om reflektionen ska rotera med formen. |
| [Size](../../aspose.cells.drawing/reflectioneffect/size/) { get; set; } | Hämtar och anger slutpositionen (längs alfa gradientrampen) för slut-alfa-värdet, i enhet procent. |
| [Transparency](../../aspose.cells.drawing/reflectioneffect/transparency/) { get; set; } | Hämtar och anger graden av startreflektionens transparens som ett värde från 0,0 (opak) till 1,0 (klar). |
| [Type](../../aspose.cells.drawing/reflectioneffect/type/) { get; set; } | Hämtar och anger den förinställda reflektionseffekten. |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassReflectionEffectDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en exempelform
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 150);

            // Ställ in egenskaper för reflektionseffekt
            ReflectionEffect reflection = shape.Reflection;
            reflection.Size = 90;
            reflection.Blur = 30;
            reflection.Transparency = 0.5;
            reflection.Distance = 10;

            // Visa reflektionsegenskaper
            Console.WriteLine("Reflection Size: " + reflection.Size);
            Console.WriteLine("Reflection Blur: " + reflection.Blur);
            Console.WriteLine("Reflection Transparency: " + reflection.Transparency);
            Console.WriteLine("Reflection Distance: " + reflection.Distance);

            // Spara arbetsboken
            workbook.Save("ReflectionEffectDemo.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


