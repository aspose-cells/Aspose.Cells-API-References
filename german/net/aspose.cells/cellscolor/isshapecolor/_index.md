---
title: "CellsColor.IsShapeColor"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "CellsColor‑Eigenschaft. Gibt die Farbe zurück und legt sie fest, die auf Zelle oder Form angewendet werden soll."
type: docs
url: /de/net/aspose.cells/cellscolor/isshapecolor/
---
## CellsColor.IsShapeColor property

Liest und setzt die Farbe, die auf Zelle oder Form angewendet werden soll.

```csharp
public bool IsShapeColor { get; set; }
```

### Hinweise

Der Ausdruck der Farbe von Zelle und Form ist unterschiedlich. Zum Beispiel wird die Themenfarbe mit demselben Tönungswert in der Zelle und der Form nicht gleich sein.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class CellsColorPropertyIsShapeColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstelle eine CellsColor‑Instanz und setze IsShapeColor.
            CellsColor cellsColor = workbook.CreateCellsColor();
            cellsColor.IsShapeColor = true;
            cellsColor.Color = Color.Green;

            // Wende die Farbe auf eine Form an.
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 100, 100);
            shape.Fill.FillType = FillType.Solid;
            shape.Fill.SolidFill.Color = cellsColor.Color;  // Use the Color property instead of CellsColor directly

            // Speichere die Arbeitsmappe
            workbook.Save("CellsColorIsShapeColorDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [CellsColor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


