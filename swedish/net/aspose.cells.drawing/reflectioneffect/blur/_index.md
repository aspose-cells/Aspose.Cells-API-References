---
title: "ReflectionEffect.Blur"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ReflectionEffect property. Hämtar och anger blur‑radien i enheter av punkter"
type: docs
url: /sv/net/aspose.cells.drawing/reflectioneffect/blur/
---
## ReflectionEffect.Blur property

Hämtar och anger oskarphetsradien, i enheter av punkter.

```csharp
public double Blur { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ReflectionEffectPropertyBlurDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till en rektangelform
            Aspose.Cells.Drawing.Shape rectangle = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 100, 100);
            
            // Kom åt reflektionseffekt
            Aspose.Cells.Drawing.ReflectionEffect reflection = rectangle.Reflection;
            
            // Ställ in reflektionstyp och egenskaper
            reflection.Type = Aspose.Cells.Drawing.ReflectionEffectType.HalfReflectionTouching;
            reflection.Blur = 0.5; // Demonstrate Blur property
            reflection.Transparency = 0.5;
            reflection.Size = 55;
            reflection.Distance = 0;
            
            // Spara arbetsboken
            workbook.Save("ReflectionEffectDemo.xlsx");
            
            // Visa blur‑värdet
            Console.WriteLine("Reflection Blur: " + reflection.Blur);
        }
    }
}
```

### Se även

* class [ReflectionEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


