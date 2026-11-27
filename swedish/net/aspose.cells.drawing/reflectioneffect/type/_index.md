---
title: "ReflectionEffect.Type"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ReflectionEffect property. Hämtar och anger den förinställda reflektionseffekten"
type: docs
url: /sv/net/aspose.cells.drawing/reflectioneffect/type/
---
## ReflectionEffect.Type property

Hämtar och anger den förinställda reflektionseffekten.

```csharp
public ReflectionEffectType Type { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ReflectionEffectPropertyTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till en rektangelform
            Shape shape = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 100, 100);
            
            // Hämta reflektionseffekt
            ReflectionEffect reflection = shape.Reflection;
            
            // Demonstrera Type‑egenskapen
            Console.WriteLine("Initial reflection type: " + reflection.Type);
            
            // Ändra reflektionstyp
            reflection.Type = ReflectionEffectType.HalfReflectionTouching;
            Console.WriteLine("Updated reflection type: " + reflection.Type);
            
            // Ställ in andra reflektionsegenskaper
            reflection.Transparency = 0.5;
            reflection.Size = 55;
            reflection.Blur = 0.5;
            reflection.Distance = 0;
            
            // Spara arbetsboken
            workbook.Save("ReflectionEffectDemo.xlsx");
            
            Console.WriteLine("Demo completed successfully.");
        }
    }
}
```

### Se även

* enum [ReflectionEffectType](../../reflectioneffecttype/)
* class [ReflectionEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


