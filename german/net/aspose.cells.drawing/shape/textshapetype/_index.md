---
title: "Shape.TextShapeType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Shape-Eigenschaft. Liest und setzt den voreingestellten Text-Shape-Typ"
type: docs
url: /de/net/aspose.cells.drawing/shape/textshapetype/
---
## Shape.TextShapeType property

Liest und setzt den voreingestellten Textformtyp.

```csharp
public AutoShapeType TextShapeType { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyTextShapeTypeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge ein Rechteck shape mit korrekten Parametern hinzu
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 150, 0);

            // Überprüfen und festlegen von TextShapeType, falls unbekannt
            if (shape.TextShapeType == AutoShapeType.Unknown)
            {
                shape.TextShapeType = AutoShapeType.Rectangle;
            }

            // Gib den TextShapeType der Form aus
            Console.WriteLine("Shape TextShapeType: " + shape.TextShapeType);
        }
    }
}
```

### Siehe auch

* enum [AutoShapeType](../../autoshapetype/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


