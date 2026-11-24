---
title: "Shape.Title"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Shape-Eigenschaft. Gibt die Titelbeschriftung des aktuellen Shape-Objekts an"
type: docs
url: /de/net/aspose.cells.drawing/shape/title/
---
## Shape.Title property

Gibt den Titel (Beschriftung) des aktuellen Formobjekts an.

```csharp
public string Title { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyTitleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge eine Rechteckform mit allen erforderlichen Parametern hinzu
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 1, 100, 200);

            // Setzen Sie den Titel des Shape
            shape.Title = "title1";

            // Überprüfen Sie, ob der Titel gesetzt wurde
            Console.WriteLine("Shape title: " + shape.Title);
        }
    }
}
```

### Siehe auch

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


