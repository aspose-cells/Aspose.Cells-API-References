---
title: "ReflectionEffect.RotWithShape"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ReflectionEffect property. Hämtar och anger om reflektionen ska rotera med formen"
type: docs
url: /sv/net/aspose.cells.drawing/reflectioneffect/rotwithshape/
---
## ReflectionEffect.RotWithShape property

Hämtar och anger om reflektionen ska rotera med formen.

```csharp
public bool RotWithShape { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ReflectionEffectPropertyRotWithShapeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en form i kalkylbladet
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 150);

            // Skapa och tillämpa reflektionseffekt
            ReflectionEffect reflection = shape.Reflection;
            reflection.Type = ReflectionEffectType.FullReflection4PtOffset;
            reflection.Blur = 5;
            reflection.Distance = 10;
            reflection.Transparency = 0.3;

            // Visa aktuellt RotWithShape‑värde
            Console.WriteLine("Current RotWithShape value: " + reflection.RotWithShape);

            // Ställ in RotWithShape till true
            reflection.RotWithShape = true;
            Console.WriteLine("RotWithShape set to: " + reflection.RotWithShape);

            // Rotera formen för att demonstrera effekten
            shape.RotationAngle = 45;

            // Spara arbetsboken
            workbook.Save("ReflectionEffectRotWithShapeDemo.xlsx");
        }
    }
}
```

### Se även

* class [ReflectionEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


