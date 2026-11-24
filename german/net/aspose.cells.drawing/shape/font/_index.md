---
title: "Shape.Font"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Shape-Eigenschaft. Gibt die Schriftart der Form an"
type: docs
url: /de/net/aspose.cells.drawing/shape/font/
---
## Shape.Font property

Stellt die Schriftart des Shapes dar.

```csharp
public Font Font { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using System.Drawing;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyFontDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge dem Arbeitsblatt eine Form hinzu
            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 0, 0);

            // Greife auf die Schriftarteigenschaften der Form zu und ändere sie
            Aspose.Cells.Font font = shape.Font;
            font.Name = "Arial";
            font.Size = 12;
            font.Color = Color.Red;

            // Speichere die Arbeitsmappe
            workbook.Save("ShapeFontDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Font](../../../aspose.cells/font/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


