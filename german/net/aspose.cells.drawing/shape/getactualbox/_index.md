---
title: "Shape.GetActualBox"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Shape Methode. Gibt die tatsächliche Position und Größe der Form zurück, nachdem Drehung, Spiegelung usw. angewendet wurden."
type: docs
url: /de/net/aspose.cells.drawing/shape/getactualbox/
---
## Shape.GetActualBox method

Lese die tatsächliche Position und Größe der Form (nach Anwendung von Drehung, Spiegelung usw.).

```csharp
public float[] GetActualBox()
```

### Rückgabewert

Gibt die Position und Größe in der Reihenfolge x, y, w, h zurück

### Hinweise

Hinweis: Die Schnittstelle ist nicht vollständig funktionsfähig, insbesondere sind die Positionsinformationen nicht korrekt. Es wird empfohlen, diese Schnittstelle nicht zu verwenden, bis die Funktion vollständig ist.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodGetActualBoxDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Rechteckform hinzufügen
            Shape rectangle = worksheet.Shapes.AddRectangle(10, 10, 100, 80, 0, 0);

            // Erhalte die tatsächlichen Boxabmessungen der Form
            float[] box = rectangle.GetActualBox();

            // Gib die Boxabmessungen aus
            Console.WriteLine("Actual Box Dimensions:");
            Console.WriteLine($"Left: {box[0]}");
            Console.WriteLine($"Top: {box[1]}");
            Console.WriteLine($"Right: {box[2]}");
            Console.WriteLine($"Bottom: {box[3]}");

            // Speichere die Arbeitsmappe
            workbook.Save("ShapeGetActualBoxDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


