---
title: "Shape.TextDirection"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Shape-Eigenschaft. Gibt die Richtung des Textflusses für dieses Objekt zurück bzw. setzt sie"
type: docs
url: /de/net/aspose.cells.drawing/shape/textdirection/
---
## Shape.TextDirection property

Liest/Setzt die Richtung des Textflusses für dieses Objekt.

```csharp
public TextDirectionType TextDirection { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyTextDirectionDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie eine Textfeldform hinzu
            Shape shape = worksheet.Shapes.AddTextBox(1, 0, 0, 100, 100, 100);
            shape.Text = "Sample Text";

            // Setze und demonstriere die TextDirection-Eigenschaft
            shape.TextDirection = TextDirectionType.Context;
            Console.WriteLine("Initial TextDirection: " + shape.TextDirection);

            // Ändere die Textausrichtung
            shape.TextDirection = TextDirectionType.LeftToRight;
            Console.WriteLine("Updated TextDirection: " + shape.TextDirection);

            // Speichere die Arbeitsmappe
            workbook.Save("TextDirectionDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [TextDirectionType](../../../aspose.cells/textdirectiontype/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


