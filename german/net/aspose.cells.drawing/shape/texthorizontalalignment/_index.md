---
title: "Shape.TextHorizontalAlignment"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Shape-Eigenschaft. Liest und setzt den horizontalen Ausrichtungstyp des Textes im shape"
type: docs
url: /de/net/aspose.cells.drawing/shape/texthorizontalalignment/
---
## Shape.TextHorizontalAlignment property

Liest und setzt den horizontalen Ausrichtungstyp des Textes in der Form.

```csharp
public TextAlignmentType TextHorizontalAlignment { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyTextHorizontalAlignmentDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Rechteckform hinzufügen
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 0);

            // Text und Ausrichtung festlegen
            shape.Text = "Sample Text";
            shape.TextHorizontalAlignment = TextAlignmentType.Center;

            // Ändere die Ausrichtung, wenn sie derzeit unten ist
            if (shape.TextHorizontalAlignment == TextAlignmentType.Bottom)
            {
                shape.TextHorizontalAlignment = TextAlignmentType.Center;
            }

            // Speichere die Arbeitsmappe
            workbook.Save("ShapeTextAlignmentDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [TextAlignmentType](../../../aspose.cells/textalignmenttype/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


