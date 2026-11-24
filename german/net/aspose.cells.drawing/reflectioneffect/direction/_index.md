---
title: "ReflectionEffect.Direction"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ReflectionEffect-Eigenschaft. Gibt die Richtung der Alpha‑Verlaufsrampe relativ zur Form zurück und legt sie fest"
type: docs
url: /de/net/aspose.cells.drawing/reflectioneffect/direction/
---
## ReflectionEffect.Direction property

Ermittelt und setzt die Richtung der Alpha-Verlaufsrampe relativ zur Form selbst.

```csharp
public double Direction { get; set; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge eine Form hinzu, um den Reflexionseffekt anzuwenden
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 150);
            
            // Hole den Reflexionseffekt der Form
            ReflectionEffect reflection = shape.Reflection;
            
            // Aktuellen Direction-Wert anzeigen
            Console.WriteLine("Current Direction value: " + reflection.Direction);
            
            // Setze neuen Direction-Wert (90 Grad)
            reflection.Direction = 90;
            Console.WriteLine("New Direction value: " + reflection.Direction);
            
            // Konfiguriere weitere Reflexionseigenschaften für bessere Sichtbarkeit
            reflection.Type = ReflectionEffectType.TightReflectionTouching;
            reflection.Transparency = 0.5;
            reflection.Size = 50;
            reflection.Blur = 5;
            
            // Speichere die Arbeitsmappe, um den Reflexionseffekt zu sehen
            workbook.Save("ReflectionEffectDirectionDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ReflectionEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


