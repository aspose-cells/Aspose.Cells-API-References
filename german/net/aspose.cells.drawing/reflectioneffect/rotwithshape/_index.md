---
title: "ReflectionEffect.RotWithShape"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ReflectionEffect-Eigenschaft. Gibt an, ob die Reflexion mit der Form rotieren soll, und legt dies fest"
type: docs
url: /de/net/aspose.cells.drawing/reflectioneffect/rotwithshape/
---
## ReflectionEffect.RotWithShape property

Ermittelt und setzt, ob die Reflexion mit der Form rotieren soll.

```csharp
public bool RotWithShape { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ReflectionEffectPropertyRotWithShapeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge dem Arbeitsblatt eine Form hinzu
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 150);

            // Erstellen und Anwenden des Reflexionseffekts
            ReflectionEffect reflection = shape.Reflection;
            reflection.Type = ReflectionEffectType.FullReflection4PtOffset;
            reflection.Blur = 5;
            reflection.Distance = 10;
            reflection.Transparency = 0.3;

            // Aktuellen RotWithShape-Wert anzeigen
            Console.WriteLine("Current RotWithShape value: " + reflection.RotWithShape);

            // RotWithShape auf true setzen
            reflection.RotWithShape = true;
            Console.WriteLine("RotWithShape set to: " + reflection.RotWithShape);

            // Rotieren Sie die Form, um den Effekt zu demonstrieren
            shape.RotationAngle = 45;

            // Speichere die Arbeitsmappe
            workbook.Save("ReflectionEffectRotWithShapeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ReflectionEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


