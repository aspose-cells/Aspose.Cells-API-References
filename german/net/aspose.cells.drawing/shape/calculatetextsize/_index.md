---
title: "Shape.CalculateTextSize"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Shape-Methode. Textbereich neu berechnen"
type: docs
url: /de/net/aspose.cells.drawing/shape/calculatetextsize/
---
## Shape.CalculateTextSize method

Berechne den Textbereich neu.

```csharp
public int[] CalculateTextSize()
```

### Rückgabewert

Größe des Textes in einem Array (Breite und Höhe).

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodCalculateTextSizeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieltext zu Zelle A1 hinzufügen
            worksheet.Cells["A1"].PutValue("Sample Text for Size Calculation");

            // Erstelle ein Rechteck-Shape mit allen erforderlichen Parametern
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 1, 100, 200);

            // Text dem Shape zuweisen
            shape.Text = "This is a test string to calculate text size";

            // Berechne die Textgröße
            int[] size = shape.CalculateTextSize();

            // Ergebnisse ausgeben
            Console.WriteLine($"Calculated text size - Width: {size[0]}, Height: {size[1]}");
        }
    }
}
```

### Siehe auch

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


