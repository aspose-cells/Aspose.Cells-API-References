---
title: "ReflectionEffect.Distance"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ReflectionEffect-Eigenschaft. Gibt an, wie weit der Schatten entfernt wird, und legt ihn fest, angegeben in Punkten"
type: docs
url: /de/net/aspose.cells.drawing/reflectioneffect/distance/
---
## ReflectionEffect.Distance property

Ermittelt und setzt, wie weit der Schatten entfernt ist, in Punkt-Einheiten.

```csharp
public double Distance { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ReflectionEffectPropertyDistanceDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie eine Form hinzu, um die Reflexion zu testen – feste Parameter, die zur Methodensignatur passen
            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 0, 0);

            // Spiegelungseigenschaften festlegen
            ReflectionEffect reflection = shape.Reflection;
            reflection.Type = ReflectionEffectType.HalfReflection4PtOffset;
            reflection.Transparency = 0.5;
            reflection.Size = 55.5;
            reflection.Blur = 0.5;
            reflection.Distance = 4; // Demonstrating Distance property

            // Speichern und neu laden, um die Persistenz zu überprüfen
            string outputPath = "ReflectionEffectDemo.xlsx";
            workbook.Save(outputPath);

            // Neu laden, um zu überprüfen
            Workbook loadedWorkbook = new Workbook(outputPath);
            Shape loadedShape = loadedWorkbook.Worksheets[0].Shapes[0];
            ReflectionEffect loadedReflection = loadedShape.Reflection;

            Console.WriteLine("Original Distance: " + reflection.Distance);
            Console.WriteLine("Loaded Distance: " + loadedReflection.Distance);
        }
    }
}
```

### Siehe auch

* class [ReflectionEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


