---
title: "ReflectionEffect.Distance"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ReflectionEffect property. Hämtar och anger hur långt skuggan ska förskjutas i enheter av punkter"
type: docs
url: /sv/net/aspose.cells.drawing/reflectioneffect/distance/
---
## ReflectionEffect.Distance property

Hämtar och anger hur långt skuggan ska förskjutas, i enheter av punkter.

```csharp
public double Distance { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ReflectionEffectPropertyDistanceDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en form för att testa reflektion – fasta parametrar för att matcha metodsignaturen
            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 0, 0);

            // Ställ in reflektionsegenskaper
            ReflectionEffect reflection = shape.Reflection;
            reflection.Type = ReflectionEffectType.HalfReflection4PtOffset;
            reflection.Transparency = 0.5;
            reflection.Size = 55.5;
            reflection.Blur = 0.5;
            reflection.Distance = 4; // Demonstrating Distance property

            // Spara och ladda om för att verifiera beständighet
            string outputPath = "ReflectionEffectDemo.xlsx";
            workbook.Save(outputPath);

            // Ladda om för att verifiera
            Workbook loadedWorkbook = new Workbook(outputPath);
            Shape loadedShape = loadedWorkbook.Worksheets[0].Shapes[0];
            ReflectionEffect loadedReflection = loadedShape.Reflection;

            Console.WriteLine("Original Distance: " + reflection.Distance);
            Console.WriteLine("Loaded Distance: " + loadedReflection.Distance);
        }
    }
}
```

### Se även

* class [ReflectionEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


