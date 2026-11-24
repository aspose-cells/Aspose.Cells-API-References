---
title: "Enum ReflectionEffectType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Drawing.ReflectionEffectType-Enum. Stellt den Effekttyp der Reflexion dar"
type: docs
url: /de/net/aspose.cells.drawing/reflectioneffecttype/
---
## ReflectionEffectType enumeration

Stellt den Effekt‑Typ der Reflexion dar.

```csharp
public enum ReflectionEffectType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| None | `0` | Kein Reflexionseffekt. |
| Custom | `1` | Benutzerdefinierter Reflexionseffekt. |
| TightReflectionTouching | `2` | Enge Reflexion, berührend. |
| HalfReflectionTouching | `3` | Halbe Reflexion, berührend. |
| FullReflectionTouching | `4` | Vollständige Reflexion, berührend. |
| TightReflection4PtOffset | `5` | Enge Reflexion, 4 pt Versatz. |
| HalfReflection4PtOffset | `6` | Halbe Reflexion, 4 pt Versatz. |
| FullReflection4PtOffset | `7` | Vollständige Reflexion, 4 pt Versatz. |
| TightReflection8PtOffset | `8` | Enge Spiegelung, 8 pt Versatz. |
| HalfReflection8PtOffset | `9` | Halbe Spiegelung, 8 pt Versatz. |
| FullReflection8PtOffset | `10` | Vollständige Spiegelung, 8 pt Versatz. |

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Rechteckform hinzufügen
            Shape rectangle = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 100, 100);
            
            // Den Spiegelungseffekt abrufen
            ReflectionEffect reflection = rectangle.Reflection;
            
            // Spiegelungseigenschaften festlegen
            reflection.Type = ReflectionEffectType.HalfReflectionTouching;
            reflection.Transparency = 0.5;
            reflection.Size = 55;
            reflection.Blur = 0.5;
            reflection.Distance = 0;
            
            // Speichere die Arbeitsmappe
            workbook.Save("DrawingClassReflectionEffectTypeDemo.xlsx");
            
            Console.WriteLine("Reflection effect demo completed successfully.");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


