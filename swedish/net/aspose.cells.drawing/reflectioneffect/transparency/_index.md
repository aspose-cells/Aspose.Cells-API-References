---
title: "ReflectionEffect.Transparency"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ReflectionEffect-egenskap. Hämtar och anger graden av den initiala reflektionens transparens som ett värde från 0.0 ogenomskinlig till 1.0 klar"
type: docs
url: /sv/net/aspose.cells.drawing/reflectioneffect/transparency/
---
## ReflectionEffect.Transparency property

Hämtar och anger graden av startreflektionens transparens som ett värde från 0,0 (opak) till 1,0 (klar).

```csharp
public double Transparency { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ReflectionEffectPropertyTransparencyDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Lägg till en rektangelform i det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            Aspose.Cells.Drawing.Shape rectangle = worksheet.Shapes.AddRectangle(0, 0, 100, 100, 200, 150);
            
            // Hämta reflektionseffekten och ställ in dess egenskaper
            Aspose.Cells.Drawing.ReflectionEffect reflection = rectangle.Reflection;
            reflection.Type = Aspose.Cells.Drawing.ReflectionEffectType.HalfReflectionTouching;
            reflection.Transparency = 0.5; // Demonstrate transparency property
            reflection.Size = 55;
            reflection.Blur = 0.5;
            reflection.Distance = 0;
            
            // Spara arbetsboken
            workbook.Save("ReflectionEffectDemo.xlsx");
            
            // Verifiera de sparade egenskaperna
            Workbook loadedWorkbook = new Workbook("ReflectionEffectDemo.xlsx");
            Aspose.Cells.Drawing.ReflectionEffect loadedReflection = loadedWorkbook.Worksheets[0].Shapes[0].Reflection;
            
            Console.WriteLine("Reflection Type: " + loadedReflection.Type);
            Console.WriteLine("Transparency: " + loadedReflection.Transparency);
            Console.WriteLine("Size: " + loadedReflection.Size);
            Console.WriteLine("Blur: " + loadedReflection.Blur);
            Console.WriteLine("Distance: " + loadedReflection.Distance);
        }
    }
}
```

### Se även

* class [ReflectionEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


