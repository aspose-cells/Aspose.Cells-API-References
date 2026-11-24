---
title: "Shape.Glow"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Shape-Eigenschaft. Stellt ein GlowEffect-Objekt dar, das den Leuchteffekt für das Diagrammelement oder Shape angibt."
type: docs
url: /de/net/aspose.cells.drawing/shape/glow/
---
## Shape.Glow property

Stellt ein [`GlowEffect`](../../gloweffect/)-Objekt dar, das den Leuchteffekt für das Diagrammelement oder Shape spezifiziert.

```csharp
public GlowEffect Glow { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyGlowDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Rechteckform hinzufügen
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 150);

            // Auf den Glow-Effekt zugreifen
            GlowEffect glow = shape.Glow;

            // Glow-Eigenschaften festlegen
            CellsColor color = workbook.CreateCellsColor();
            color.Color = System.Drawing.Color.Purple;
            glow.Color = color;
            glow.Size = 10; // 10 point radius
            glow.Transparency = 0.5; // 50% transparency

            // Speichere die Arbeitsmappe
            workbook.Save("ShapeGlowDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [GlowEffect](../../gloweffect/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


