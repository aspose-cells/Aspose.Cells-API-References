---
title: "Shape.Glow"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Shape. Rappresenta un oggetto GlowEffect che specifica l'effetto bagliore per l'elemento del grafico o la forma"
type: docs
url: /it/net/aspose.cells.drawing/shape/glow/
---
## Shape.Glow property

Rappresenta un oggetto [`GlowEffect`](../../gloweffect/) che specifica l'effetto bagliore per l'elemento del grafico o la forma.

```csharp
public GlowEffect Glow { get; }
```

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma rettangolare
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 150);

            // Accedi all'effetto bagliore
            GlowEffect glow = shape.Glow;

            // Imposta le proprietà del bagliore
            CellsColor color = workbook.CreateCellsColor();
            color.Color = System.Drawing.Color.Purple;
            glow.Color = color;
            glow.Size = 10; // 10 point radius
            glow.Transparency = 0.5; // 50% transparency

            // Salva la cartella di lavoro
            workbook.Save("ShapeGlowDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [GlowEffect](../../gloweffect/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


