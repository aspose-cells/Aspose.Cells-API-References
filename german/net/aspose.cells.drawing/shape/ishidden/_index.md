---
title: "Shape.IsHidden"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Shape-Eigenschaft. Gibt an, ob das Objekt sichtbar ist"
type: docs
url: /de/net/aspose.cells.drawing/shape/ishidden/
---
## Shape.IsHidden property

Gibt an, ob das Objekt sichtbar ist.

```csharp
public bool IsHidden { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyIsHiddenDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge dem Arbeitsblatt eine Form hinzu
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 0);

            // Setze die IsHidden-Eigenschaft auf false (sichtbar)
            shape.IsHidden = false;
            Console.WriteLine("Shape is visible: " + !shape.IsHidden);

            // Setze die IsHidden-Eigenschaft auf true (verborgen)
            shape.IsHidden = true;
            Console.WriteLine("Shape is hidden: " + shape.IsHidden);
        }
    }
}
```

### Siehe auch

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


