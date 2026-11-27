---
title: "ReflectionEffect.Direction"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ReflectionEffect-egenskap. Hämtar och anger riktningen för alfa-gradientens lutning i förhållande till själva formen"
type: docs
url: /sv/net/aspose.cells.drawing/reflectioneffect/direction/
---
## ReflectionEffect.Direction property

Hämtar och anger riktningen för alfa gradientrampen relativt formen själv.

```csharp
public double Direction { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ReflectionEffectPropertyDirectionDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en form för att tillämpa reflektionseffekt
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 150);
            
            // Hämta reflektionseffekten för formen
            ReflectionEffect reflection = shape.Reflection;
            
            // Visa aktuellt Direction-värde
            Console.WriteLine("Current Direction value: " + reflection.Direction);
            
            // Ange nytt Direction-värde (90 grader)
            reflection.Direction = 90;
            Console.WriteLine("New Direction value: " + reflection.Direction);
            
            // Konfigurera andra reflektionsegenskaper för bättre synlighet
            reflection.Type = ReflectionEffectType.TightReflectionTouching;
            reflection.Transparency = 0.5;
            reflection.Size = 50;
            reflection.Blur = 5;
            
            // Spara arbetsboken för att se reflektionseffekten
            workbook.Save("ReflectionEffectDirectionDemo.xlsx");
        }
    }
}
```

### Se även

* class [ReflectionEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


