---
title: "Shape.IsTextWrapped"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Shape-Eigenschaft. Gibt den Textumbruchtyp der Form zurück und legt ihn fest, die Text enthält."
type: docs
url: /de/net/aspose.cells.drawing/shape/istextwrapped/
---
## Shape.IsTextWrapped property

Ermittelt und setzt den Zeilenumbruchtyp des Textes in der Form, die Text enthält.

```csharp
public bool IsTextWrapped { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyIsTextWrappedDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge eine Form hinzu und setze etwas Text.
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 0);
            shape.Text = "This is a sample text that will demonstrate text wrapping functionality";

            // Demonstration der IsTextWrapped-Eigenschaft
            Console.WriteLine("Initial IsTextWrapped value: " + shape.IsTextWrapped);
            
            // Schalte den Textumbruch um.
            shape.IsTextWrapped = !shape.IsTextWrapped;
            Console.WriteLine("After toggle, IsTextWrapped value: " + shape.IsTextWrapped);

            // Speichere die Arbeitsmappe
            workbook.Save("ShapeTextWrappingDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


