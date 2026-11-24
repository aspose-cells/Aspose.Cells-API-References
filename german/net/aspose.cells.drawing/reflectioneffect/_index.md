---
title: "Klasse ReflectionEffect"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Drawing.ReflectionEffect-Klasse. Diese Klasse definiert einen Reflexionseffekt"
type: docs
url: /de/net/aspose.cells.drawing/reflectioneffect/
---
## ReflectionEffect class

Diese Klasse gibt einen Reflexionseffekt an.

```csharp
public class ReflectionEffect
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Blur](../../aspose.cells.drawing/reflectioneffect/blur/) { get; set; } | Ermittelt und setzt den Unschärferadius, in Punkt-Einheiten. |
| [Direction](../../aspose.cells.drawing/reflectioneffect/direction/) { get; set; } | Ermittelt und setzt die Richtung der Alpha-Verlaufsrampe relativ zur Form selbst. |
| [Distance](../../aspose.cells.drawing/reflectioneffect/distance/) { get; set; } | Ermittelt und setzt, wie weit der Schatten entfernt ist, in Punkt-Einheiten. |
| [FadeDirection](../../aspose.cells.drawing/reflectioneffect/fadedirection/) { get; set; } | Ermittelt und setzt die Richtung, um die Reflexion zu versetzen. |
| [RotWithShape](../../aspose.cells.drawing/reflectioneffect/rotwithshape/) { get; set; } | Ermittelt und setzt, ob die Reflexion mit der Form rotieren soll. |
| [Size](../../aspose.cells.drawing/reflectioneffect/size/) { get; set; } | Ermittelt und setzt die Endposition (entlang der Alpha-Verlaufsrampe) des End-Alpha-Werts, in Prozent. |
| [Transparency](../../aspose.cells.drawing/reflectioneffect/transparency/) { get; set; } | Ermittelt und setzt den Grad der Anfangs-Reflexions-Transparenz als Wert von 0,0 (undurchsichtig) bis 1,0 (klar). |
| [Type](../../aspose.cells.drawing/reflectioneffect/type/) { get; set; } | Ermittelt und setzt den voreingestellten Reflexionseffekt. |

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Eine Beispiel-Form hinzufügen
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 150);

            // Reflexionseffekt-Eigenschaften festlegen
            ReflectionEffect reflection = shape.Reflection;
            reflection.Size = 90;
            reflection.Blur = 30;
            reflection.Transparency = 0.5;
            reflection.Distance = 10;

            // Reflexionseigenschaften anzeigen
            Console.WriteLine("Reflection Size: " + reflection.Size);
            Console.WriteLine("Reflection Blur: " + reflection.Blur);
            Console.WriteLine("Reflection Transparency: " + reflection.Transparency);
            Console.WriteLine("Reflection Distance: " + reflection.Distance);

            // Speichere die Arbeitsmappe
            workbook.Save("ReflectionEffectDemo.xlsx");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


