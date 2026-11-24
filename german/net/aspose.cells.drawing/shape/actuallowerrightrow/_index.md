---
title: "Shape.ActualLowerRightRow"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Shape-Eigenschaft. Gibt die tatsächliche untere Zeile zurück"
type: docs
url: /de/net/aspose.cells.drawing/shape/actuallowerrightrow/
---
## Shape.ActualLowerRightRow property

Erhalte die tatsächliche untere Zeile.

```csharp
public int ActualLowerRightRow { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyActualLowerRightRowDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge eine Beispiel-Form (Rechteck) hinzu
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 150, 100);

            // Erhalte die tatsächliche untere rechte Zeile der Form
            int actualLowerRightRow = shape.ActualLowerRightRow;

            // Gib das Ergebnis aus
            Console.WriteLine("Actual Lower Right Row of the shape: " + actualLowerRightRow);
        }
    }
}
```

### Siehe auch

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


