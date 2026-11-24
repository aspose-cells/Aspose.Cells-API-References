---
title: "ReflectionEffect.FadeDirection"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ReflectionEffect-Eigenschaft. Gibt die Richtung zum Versetzen der Reflexion zurück und legt sie fest"
type: docs
url: /de/net/aspose.cells.drawing/reflectioneffect/fadedirection/
---
## ReflectionEffect.FadeDirection property

Ermittelt und setzt die Richtung, um die Reflexion zu versetzen.

```csharp
public double FadeDirection { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ReflectionEffectPropertyFadeDirectionDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge eine Form hinzu, um den Reflexionseffekt anzuwenden
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 100);

            // Hole den Reflexionseffekt der Form
            ReflectionEffect reflection = shape.Reflection;

            // Zeige den aktuellen FadeDirection-Wert an
            Console.WriteLine("Current FadeDirection value: " + reflection.FadeDirection);

            // Setze neuen FadeDirection-Wert (90 Grad)
            reflection.FadeDirection = 90;
            Console.WriteLine("New FadeDirection value: " + reflection.FadeDirection);

            // Konfiguriere weitere Reflexionseigenschaften für bessere Sichtbarkeit
            reflection.Type = ReflectionEffectType.TightReflectionTouching;
            reflection.Transparency = 0.5;
            reflection.Size = 50;
            reflection.Blur = 5;
            reflection.Distance = 10;

            // Speichern Sie die Arbeitsmappe, um den Effekt zu sehen
            workbook.Save("ReflectionEffectFadeDirectionDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ReflectionEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


