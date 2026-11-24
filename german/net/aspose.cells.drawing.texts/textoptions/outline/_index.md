---
title: "TextOptions.Outline"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "TextOptions-Eigenschaft. Stellt das Umrissformat des Textes dar"
type: docs
url: /de/net/aspose.cells.drawing.texts/textoptions/outline/
---
## TextOptions.Outline property

Stellt das Umrissformat des Textes dar.

```csharp
public LineFormat Outline { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class TextOptionsPropertyOutlineDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie eine Form mit Text hinzu.
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 200, 100);
            shape.Text = "Sample Text";

            // Zugriff auf Textoptionen
            TextOptions textOptions = shape.TextOptions;

            // Umrisseigenschaften konfigurieren
            LineFormat outline = textOptions.Outline;
            outline.Weight = 2.48; // Set outline weight
            outline.DashStyle = MsoLineDashStyle.Solid; // Set line style
            outline.CompoundType = MsoLineStyle.Single; // Set compound type

            // Speichere die Arbeitsmappe
            workbook.Save("TextOutlineDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [LineFormat](../../../aspose.cells.drawing/lineformat/)
* class [TextOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


