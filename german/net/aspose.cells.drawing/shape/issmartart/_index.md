---
title: "Shape.IsSmartArt"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Shape-Eigenschaft. Gibt an, ob die Form ein SmartArt ist"
type: docs
url: /de/net/aspose.cells.drawing/shape/issmartart/
---
## Shape.IsSmartArt property

Gibt an, ob die Form ein SmartArt ist.

```csharp
public bool IsSmartArt { get; }
```

### Hinweise

Nur für ooxml-Datei.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyIsSmartArtDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge eine SmartArt-Form hinzu (Hinweis: Aspose.Cells stellt die Erstellung von SmartArt in den aktuellen Versionen nicht direkt zur Verfügung)
            // Zur Demonstration prüfen wir vorhandene Formen
            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 0, 0);

            // Prüfe, ob die Form ein SmartArt ist
            if (shape.IsSmartArt)
            {
                Console.WriteLine("The shape is a SmartArt object");
            }
            else
            {
                Console.WriteLine("The shape is not a SmartArt object");
            }
        }
    }
}
```

### Siehe auch

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


