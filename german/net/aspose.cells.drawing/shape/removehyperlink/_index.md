---
title: "Shape.RemoveHyperlink"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Shape-Methode. Entfernt den Hyperlink der Shape"
type: docs
url: /de/net/aspose.cells.drawing/shape/removehyperlink/
---
## Shape.RemoveHyperlink method

Entfernt den Hyperlink der Form.

```csharp
public void RemoveHyperlink()
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodRemoveHyperlinkDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge eine Shape hinzu und setze den Hyperlink
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 50, 50);
            shape.AddHyperlink("https://www.aspose.com");

            // Entferne den Hyperlink
            shape.RemoveHyperlink();

            // Überprüfe, dass der Hyperlink entfernt wurde
            Console.WriteLine("Hyperlink removed: " + (shape.Hyperlink == null));

            // Speichere die Arbeitsmappe
            workbook.Save("ShapeRemoveHyperlinkDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


