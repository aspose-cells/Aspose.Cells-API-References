---
title: "Shape.Fill"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Shape Eigenschaft. Gibt ein FillFormat-Objekt zurück, das Füllformatierungs-Eigenschaften für die angegebene Form enthält."
type: docs
url: /de/net/aspose.cells.drawing/shape/fill/
---
## Shape.Fill property

Gibt ein [`FillFormat`](../fillformat/) Objekt zurück, das Füllformatierungs-Eigenschaften für die angegebene Form enthält.

```csharp
public FillFormat Fill { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyFillDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge ein Rechteck shape mit korrekten Parametern hinzu
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 0);

            // Lese das Füllformat der Form.
            FillFormat fillFmt = shape.Fill;

            // Setzen Sie eine einfarbige Füllung mit Farbe.
            fillFmt.SolidFill.Color = System.Drawing.Color.Red;

            // Transparenz festlegen
            fillFmt.Transparency = 0.5;

            // Speichere die Arbeitsmappe
            workbook.Save("ShapeFillDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [FillFormat](../../fillformat/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


