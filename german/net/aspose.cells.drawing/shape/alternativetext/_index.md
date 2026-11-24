---
title: "Shape.AlternativeText"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Shape-Eigenschaft. Gibt den beschreibenden alternativen Textstring des Shape-Objekts zurück oder legt ihn fest"
type: docs
url: /de/net/aspose.cells.drawing/shape/alternativetext/
---
## Shape.AlternativeText property

Gibt den beschreibenden (alternativen) Textstring des [`Shape`](../)-Objekts zurück oder legt ihn fest.

```csharp
public string AlternativeText { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyAlternativeTextDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Rechteckform hinzufügen
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 0);

            // Alternativen Text für das Shape festlegen
            shape.AlternativeText = "A rectangle shape with width 100 and height 200";

            // Speichere die Arbeitsmappe
            workbook.Save("ShapeAlternativeTextDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


