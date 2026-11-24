---
title: "SolidFill.Color"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SolidFill-Eigenschaft. Gibt die Farbe zurück oder legt sie fest."
type: docs
url: /de/net/aspose.cells.drawing/solidfill/color/
---
## SolidFill.Color property

Liest oder setzt die Farbe.

```csharp
public Color Color { get; set; }
```

### Beispiele

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class SolidFillPropertyColorDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Fügen Sie ein Shape dem Arbeitsblatt mit korrekten Parametern hinzu.
            Shape shape = sheet.Shapes.AddRectangle(1, 0, 1, 100, 100, 100);

            // Setzen Sie Shape-Eigenschaften mit Farbe.
            Color fillColor = Color.LightBlue;
            Color textColor = Color.DarkBlue;
            string text = "Solid Fill Demo";

            // Demonstrieren Sie die Verwendung der Color-Eigenschaft.
            shape.Fill.SolidFill.Color = fillColor;
            shape.LineFormat.ForeColor = fillColor;
            shape.Text = text;
            shape.Font.Color = textColor;

            // Speichere die Arbeitsmappe
            workbook.Save("SolidFillPropertyColorDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [SolidFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


