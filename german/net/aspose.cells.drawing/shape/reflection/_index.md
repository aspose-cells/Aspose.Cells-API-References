---
title: "Shape.Reflection"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Shape-Eigenschaft. Stellt ein ReflectionEffect-Objekt dar, das den Reflexionseffekt für das Diagrammelement oder die Form angibt."
type: docs
url: /de/net/aspose.cells.drawing/shape/reflection/
---
## Shape.Reflection property

Stellt ein [`ReflectionEffect`](../../reflectioneffect/) Objekt dar, das den Reflexionseffekt für das Diagrammelement oder die Form angibt.

```csharp
public ReflectionEffect Reflection { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyReflectionDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Rechteckform hinzufügen
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 150);

            // Spiegelungseigenschaften festlegen
            ReflectionEffect reflection = shape.Reflection;
            reflection.Blur = 5;
            reflection.Distance = 10;
            reflection.Direction = 90;
            reflection.FadeDirection = 90;
            reflection.Size = 50;
            reflection.Transparency = 0.5;
            reflection.Type = ReflectionEffectType.None;

            // Speichere die Arbeitsmappe
            workbook.Save("ShapeReflectionDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ReflectionEffect](../../reflectioneffect/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


