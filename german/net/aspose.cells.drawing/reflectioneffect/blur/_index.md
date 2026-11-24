---
title: "ReflectionEffect.Blur"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ReflectionEffect-Eigenschaft. Gibt den Unschärferadius zurück und legt ihn fest, angegeben in Punkten"
type: docs
url: /de/net/aspose.cells.drawing/reflectioneffect/blur/
---
## ReflectionEffect.Blur property

Ermittelt und setzt den Unschärferadius, in Punkt-Einheiten.

```csharp
public double Blur { get; set; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Rechteckform hinzufügen
            Aspose.Cells.Drawing.Shape rectangle = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 100, 100);
            
            // Auf Reflexionseffekt zugreifen
            Aspose.Cells.Drawing.ReflectionEffect reflection = rectangle.Reflection;
            
            // Reflexionstyp und -eigenschaften festlegen
            reflection.Type = Aspose.Cells.Drawing.ReflectionEffectType.HalfReflectionTouching;
            reflection.Blur = 0.5; // Demonstrate Blur property
            reflection.Transparency = 0.5;
            reflection.Size = 55;
            reflection.Distance = 0;
            
            // Speichere die Arbeitsmappe
            workbook.Save("ReflectionEffectDemo.xlsx");
            
            // Unschärfewert anzeigen
            Console.WriteLine("Reflection Blur: " + reflection.Blur);
        }
    }
}
```

### Siehe auch

* class [ReflectionEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


