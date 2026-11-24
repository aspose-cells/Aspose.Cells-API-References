---
title: "Shape.IsPrintable"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Shape-Eigenschaft. Gibt an, ob das Objekt druckbar ist. Wenn False, wird dieses Shape beim Drucken nicht ausgegeben."
type: docs
url: /de/net/aspose.cells.drawing/shape/isprintable/
---
## Shape.IsPrintable property

Gibt an, ob das Objekt druckbar ist. Wenn False, wird diese Form beim Drucken nicht ausgedruckt.

```csharp
public bool IsPrintable { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyIsPrintableDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge dem Arbeitsblatt eine Form hinzu
            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 0, 0);

            // Demonstriere die IsPrintable-Eigenschaft
            Console.WriteLine("Shape is printable initially: " + shape.IsPrintable);

            // Schalte die IsPrintable-Eigenschaft um
            shape.IsPrintable = !shape.IsPrintable;
            Console.WriteLine("Shape is printable after toggle: " + shape.IsPrintable);

            // Setze IsPrintable explizit auf false
            shape.IsPrintable = false;
            Console.WriteLine("Shape is printable after setting to false: " + shape.IsPrintable);
        }
    }
}
```

### Siehe auch

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


