---
title: "ReflectionEffect.FadeDirection"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ReflectionEffect-egenskap. Hämtar och anger riktningen för att förskjuta reflektionen"
type: docs
url: /sv/net/aspose.cells.drawing/reflectioneffect/fadedirection/
---
## ReflectionEffect.FadeDirection property

Hämtar och anger riktningen för att förskjuta reflektionen.

```csharp
public double FadeDirection { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ReflectionEffectPropertyFadeDirectionDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en form för att tillämpa reflektionseffekt
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 100);

            // Hämta reflektionseffekten för formen
            ReflectionEffect reflection = shape.Reflection;

            // Visa aktuellt FadeDirection-värde
            Console.WriteLine("Current FadeDirection value: " + reflection.FadeDirection);

            // Ange nytt FadeDirection-värde (90 grader)
            reflection.FadeDirection = 90;
            Console.WriteLine("New FadeDirection value: " + reflection.FadeDirection);

            // Konfigurera andra reflektionsegenskaper för bättre synlighet
            reflection.Type = ReflectionEffectType.TightReflectionTouching;
            reflection.Transparency = 0.5;
            reflection.Size = 50;
            reflection.Blur = 5;
            reflection.Distance = 10;

            // Spara arbetsboken för att se effekten
            workbook.Save("ReflectionEffectFadeDirectionDemo.xlsx");
        }
    }
}
```

### Se även

* class [ReflectionEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


