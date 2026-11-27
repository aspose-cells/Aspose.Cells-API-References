---
title: "Enum ReflectionEffectType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Drawing.ReflectionEffectType enum. Representerar reflektionseffektens typ"
type: docs
url: /sv/net/aspose.cells.drawing/reflectioneffecttype/
---
## ReflectionEffectType enumeration

Representerar effekttypen för reflektion.

```csharp
public enum ReflectionEffectType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| None | `0` | Ingen reflektionseffekt. |
| Custom | `1` | Anpassad reflektionseffekt. |
| TightReflectionTouching | `2` | Tät reflektion, berör. |
| HalfReflectionTouching | `3` | Halv reflektion, berör. |
| FullReflectionTouching | `4` | Full reflektion, berör. |
| TightReflection4PtOffset | `5` | Tät reflektion, 4 pt förskjutning. |
| HalfReflection4PtOffset | `6` | Halv reflektion, 4 pt förskjutning. |
| FullReflection4PtOffset | `7` | Full reflektion, 4 pt förskjutning. |
| TightReflection8PtOffset | `8` | Tät reflektion, 8 pt förskjutning. |
| HalfReflection8PtOffset | `9` | Halv reflektion, 8 pt förskjutning. |
| FullReflection8PtOffset | `10` | Full reflektion, 8 pt förskjutning. |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassReflectionEffectTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till en rektangelform
            Shape rectangle = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 100, 100);
            
            // Hämta reflektionseffekten
            ReflectionEffect reflection = rectangle.Reflection;
            
            // Ställ in reflektionsegenskaper
            reflection.Type = ReflectionEffectType.HalfReflectionTouching;
            reflection.Transparency = 0.5;
            reflection.Size = 55;
            reflection.Blur = 0.5;
            reflection.Distance = 0;
            
            // Spara arbetsboken
            workbook.Save("DrawingClassReflectionEffectTypeDemo.xlsx");
            
            Console.WriteLine("Reflection effect demo completed successfully.");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


