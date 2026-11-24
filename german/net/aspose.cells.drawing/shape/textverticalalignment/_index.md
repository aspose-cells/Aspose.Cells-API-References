---
title: "Shape.TextVerticalAlignment"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Shape-Eigenschaft. Ruft den vertikalen Ausrichtungstyp des Textes der Shape ab und legt ihn fest"
type: docs
url: /de/net/aspose.cells.drawing/shape/textverticalalignment/
---
## Shape.TextVerticalAlignment property

Liest und setzt den vertikalen Ausrichtungstyp des Textes in der Form.

```csharp
public TextAlignmentType TextVerticalAlignment { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyTextVerticalAlignmentDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Rechteckform hinzufügen
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 0);

            // Text und Ausrichtung festlegen
            shape.Text = "Vertical Alignment Demo";
            shape.TextVerticalAlignment = TextAlignmentType.Bottom;
            
            Console.WriteLine("Initial Vertical Alignment: " + shape.TextVerticalAlignment);

            // Vertikale Ausrichtung ändern
            if (shape.TextVerticalAlignment == TextAlignmentType.Bottom)
            {
                shape.TextVerticalAlignment = TextAlignmentType.Center;
            }

            Console.WriteLine("Updated Vertical Alignment: " + shape.TextVerticalAlignment);

            // Speichere die Arbeitsmappe
            workbook.Save("TextVerticalAlignmentDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [TextAlignmentType](../../../aspose.cells/textalignmenttype/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


