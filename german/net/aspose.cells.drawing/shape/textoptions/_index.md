---
title: "Shape.TextOptions"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Shape-Eigenschaft. Stellt die Texteinstellungen der Form dar"
type: docs
url: /de/net/aspose.cells.drawing/shape/textoptions/
---
## Shape.TextOptions property

Stellt die Textoptionen der Form dar.

```csharp
public TextOptions TextOptions { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyTextOptionsDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge dem Arbeitsblatt eine Form hinzu
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 150);

            // Setzen Sie den Text für das Shape
            shape.Text = "Sample Text";

            // Zugreifen und TextOptions ändern
            TextOptions opt = shape.TextOptions;
            opt.Color = Color.Blue;
            opt.Size = 8;

            // Speichere die Arbeitsmappe
            workbook.Save("ShapeTextOptionsDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [TextOptions](../../../aspose.cells.drawing.texts/textoptions/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


